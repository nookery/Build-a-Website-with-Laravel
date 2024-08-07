# Laravel Optimize

This article is still in the draft stage, so its content may change.## 简介

当你准备部署你的 Laravel 应用到生产环境时，请确保几个重要的注意点以保证你的应用能尽可能高效的运行。本文中我们将会覆盖几个重点来确保你的 Laravel 应用部署得当。

**如果是在开发环境中，不需要进行以下操作，以避免代码不生效的问题。**

## 自动加载器优化

当你准备部署应用到生产环境时，你应该对 Composer 类的自动加载映射进行优化，使得 Composer 可以很快找到指定类的正确的加载文件。

技巧：为了优化自动加载器，你应该确保你的项目代码管理从库中包含了 composer.lock 这个文件。当你的项目中包含了 composer.lock 文件，便可以很快地安装项目中需要的依赖项。

## 优化配置加载

当你准备部署应用到生产环境时，你应该部署过程中运行 config:cache Artisan 命令：

该命令会合并所有的 Laravel 配置文件到一个缓存文件，这将极大程度上减少框架加载配置值时对文件系统的访问次数。

注意：如果你在部署过程中运行了 config:cache 命令，你应该确保你仅从配置文件中调用 env 函数。一旦配置被缓存，.env 文件将不再加载并且 env 方法将会返回 null。

## 优化路由加载

如果你在构建一个拥有大量路由的大型应用，你应该确保你在部署的过程中执行 route:cache：

这个命令将会把所有的路由注册所见到一个缓存文件的单个函数调用，从而在注册上百个路由时能够提高路由注册的性能。

## 优化视图加载

当你往生产环境中部署应用时，你应该确保在部署过程中运行 view:cache：

这个命令预编译所有的 Blade 视图，因此不会按需编译，此举提高了每个返回视图的请求的性能。