# PHP

## Instruction

PHP, which stands for "Hypertext Preprocessor," is a popular server-side scripting language used for web development. In this article, we will introduce you to PHP, discuss its features and capabilities and guide you through the process of installing and using PHP on macOS.

What is PHP?is a versatile powerful scripting language commonly for web development. is especially well-su for creating dynamic web and web applications. PHP code is within HTML pages processed on the server side before being sent to client's web browser allowing for the generation dynamic content.

## What can PHP do

PHP can perform a range of tasks:

- Dynamically web pages

- Interact with to store and retrieve information

- Handle form data submitted by users

- Create and manipulate files on the server

- Implement user authentication and access

- Process and validate user input

- Generate dynamic graphics and charts

- And much more!

## Installation on macOS

### Step 1: Install Homebrew

Homebrew is a package manager for macOS that simplifies the installation of software packages. install Homebrew, open Terminal and run the following command:

### Step 2: Install PHP

Once Homebrew is installed you can install PHP by running the following command:

### Step 3: Verify Installation

To verify that PHP is installed, run the following command in Terminal:

## How to Use PHP on macOS

### Create a PHP

1. Open a text editor like Visual Studio Code or TextEdit2. Write your PHP code, for example:

3. Save the file with a .php extension, example hello.php.

### Run the PHP File

1. Open and navigate to the directory where your PHP file is saved.

2. the PHP file using the following command:

3. You should see the output `Hello, World! in the Terminal.

Congratulations! You have successfully installed PHP on your macOS and run a simple PHP script. You can now further and start building dynamic web applications using PHP.

In conclusion, PHP a powerful scripting language with a wide range of capabilities, and installing and PHP on macOS is relatively straightforward with the help of tools like Homebrew Happy coding!

## Pre-Check

Print the version:

List extensions:

## Install Extension with PECL

例如安装redis扩展。

### 1、快速安装

### 2、编译安装

****下载并解压扩展

****编译

运行php -m查看列表中是否有redis，如果没有，继续下一步。

找出当前PHP的配置文件的位置：

 /Library/Application Support/appsolute/MAMP PRO/conf/php7.4.1.ini\\nlibXML Loaded Version => 20800\\nLoaded plugins => mysqlnd,debug_trace,auth_plugin_mysql_native_password,auth_plugin_mysql_clear_password,auth_plugin_caching_sha2_password,auth_plugin_sha256_password&quot;,&quot;language&quot;:&quot;Text&quot;,&quot;runVisible&quot;:true}],&quot;activatedIndex&quot;:0}" uuid="98a95258-4cde-4a4e-b385-89226f0ffb99">可以看出配置文件是：/Library/Application Support/appsolute/MAMP PRO/conf/php7.4.1.ini 编辑配置文件，增加一行extension=mongodb.so

### 3、指定PHP版本

如果安装了多个版本的 PHP，pecl install可能将扩展安装到了其他的PHP版本中。 这时候我们可以指定编译时使用的PHP版本。

****下载并解压扩展

****编译

注意其中的phpize、php、php-config的路径。

****改PHP的配置文件

找出当前PHP的配置文件的位置：

 /Library/Application Support/appsolute/MAMP PRO/conf/php7.4.1.ini\\nlibXML Loaded Version => 20800\\nLoaded plugins => mysqlnd,debug_trace,auth_plugin_mysql_native_password,auth_plugin_mysql_clear_password,auth_plugin_caching_sha2_password,auth_plugin_sha256_password&quot;,&quot;language&quot;:&quot;Text&quot;,&quot;runVisible&quot;:true}],&quot;activatedIndex&quot;:0}" uuid="7f5d7410-2e90-494a-b329-5e6dc8eaee2b">可以看出配置文件是：/Library/Application Support/appsolute/MAMP PRO/conf/php7.4.1.ini 编辑配置文件，增加一行extension=mongodb.so

## Say Hello to PHP

Next, you will learn how to run a PHP file.

### Print the time

Open this project with Visual Studio Code

Open the terminal app by pressing Ctrl + ~

Follow the steps below to print the time.

Create a new file called time.php in the docs/php directory of this project.

Write the following code in the file:

Enter this code within the terminal app and hit enter to run:

If you see the following output, congratulations! You have successfully printed the time.

Now, you have learned how to write a PHP file and run it.

### Function

Create a new file called function.php in the docs/php directory of this project.

Write a function to print the Fibonacci sequence. Fill in the missing code.

### Array Sorting

Create a new file called array_sorting.php in the docs/php directory of this project.

Here is a function that takes two arrays and merges them into one and sort in ascending order. Fill in the missing code.

The array c should be: [1,2,3,4,5].

### HTTP Server

Create a new file called http_server.php in the docs/php directory of this project. Create a HTTP server that listens on port 8000 with this shell command:

When the user accesses the homepage, print "Hello World!".

This is the basic principle of developing web pages.