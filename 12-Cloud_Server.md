# Cloud Server

This article is still in the draft stage, so its content may change.## What is Cloud Server

Simply put, a cloud server is a computer that doesn’t shut down.

## Why do We Need a Cloud Server

As a software developer, you may need a cloud server for the following reasons:

**Deploying Applications:** Deploy your applications on a cloud server to make them accessible and usable globally.

**Collaboration and Remote Access:** Cloud servers enable team members to remotely access and collaborate on development, testing, and deployment of applications, regardless of their location

## How to Get a Cloud Server

[https://cloud.tencent.com/act/pro/free](https://cloud.tencent.com/act/pro/free)

[https://aws.amazon.com/ec2](https://aws.amazon.com/ec2)

## Install Softwares

### Update Packages

### Install Softwares

## Deploy Your Project to Cloud Server

Publish your project a cloud server so others can access it through a link like:

http://123.456.3.4:8000

![](./images/12-Cloud_Server_1.png)

### Clone Project

### Install Composer

### Install PHP Packages

Install PHP packages

### Install PHP Extensions

If the output is something like this

 it is missing from your system. Install or enable PHP's dom extension.\n  Problem 2\n    - laravel/pint is locked to version v1.16.2 and an update of this package was not requested.\n    - laravel/pint v1.16.2 requires ext-xml * -> it is missing from your system. Install or enable PHP's xml extension.\n  Problem 3\n    - phar-io/manifest is locked to version 2.0.4 and an update of this package was not requested.\n    - phar-io/manifest 2.0.4 requires ext-dom * -> it is missing from your system. Install or enable PHP's dom extension.\n  Problem 4\n    - phpunit/php-code-coverage is locked to version 11.0.5 and an update of this package was not requested.\n    - phpunit/php-code-coverage 11.0.5 requires ext-dom * -> it is missing from your system. Install or enable PHP's dom extension.\n  Problem 5\n    - phpunit/phpunit is locked to version 11.2.8 and an update of this package was not requested.\n    - phpunit/phpunit 11.2.8 requires ext-dom * -> it is missing from your system. Install or enable PHP's dom extension.\n  Problem 6\n    - sebastian/comparator is locked to version 6.0.1 and an update of this package was not requested.\n    - sebastian/comparator 6.0.1 requires ext-dom * -> it is missing from your system. Install or enable PHP's dom extension.\n  Problem 7\n    - theseer/tokenizer is locked to version 1.2.3 and an update of this package was not requested.\n    - theseer/tokenizer 1.2.3 requires ext-dom * -> it is missing from your system. Install or enable PHP's dom extension.\n  Problem 8\n    - tijsverkoyen/css-to-inline-styles v2.2.7 requires ext-dom * -> it is missing from your system. Install or enable PHP's dom extension.\n    - laravel/framework v11.16.0 requires tijsverkoyen/css-to-inline-styles ^2.2.5 -> satisfiable by tijsverkoyen/css-to-inline-styles[v2.2.7].\n    - laravel/framework is locked to version v11.16.0 and an update of this package was not requested.\n\nTo enable extensions, verify that they are enabled in your .ini files:\n    - /etc/php/8.3/cli/php.ini\n    - /etc/php/8.3/cli/conf.d/10-opcache.ini\n    - /etc/php/8.3/cli/conf.d/10-pdo.ini\n    - /etc/php/8.3/cli/conf.d/20-calendar.ini\n    - /etc/php/8.3/cli/conf.d/20-ctype.ini\n    - /etc/php/8.3/cli/conf.d/20-curl.ini\n    - /etc/php/8.3/cli/conf.d/20-exif.ini\n    - /etc/php/8.3/cli/conf.d/20-ffi.ini\n    - /etc/php/8.3/cli/conf.d/20-fileinfo.ini\n    - /etc/php/8.3/cli/conf.d/20-ftp.ini\n    - /etc/php/8.3/cli/conf.d/20-gettext.ini\n    - /etc/php/8.3/cli/conf.d/20-iconv.ini\n    - /etc/php/8.3/cli/conf.d/20-intl.ini\n    - /etc/php/8.3/cli/conf.d/20-mbstring.ini\n    - /etc/php/8.3/cli/conf.d/20-phar.ini\n    - /etc/php/8.3/cli/conf.d/20-posix.ini\n    - /etc/php/8.3/cli/conf.d/20-readline.ini\n    - /etc/php/8.3/cli/conf.d/20-shmop.ini\n    - /etc/php/8.3/cli/conf.d/20-sockets.ini\n    - /etc/php/8.3/cli/conf.d/20-sysvmsg.ini\n    - /etc/php/8.3/cli/conf.d/20-sysvsem.ini\n    - /etc/php/8.3/cli/conf.d/20-sysvshm.ini\n    - /etc/php/8.3/cli/conf.d/20-tokenizer.ini\n    - /etc/php/8.3/cli/conf.d/20-zip.ini\nYou can also run `php --ini` in a terminal to see which files are used by PHP in CLI mode.\nAlternatively, you can run Composer with `--ignore-platform-req=ext-dom --ignore-platform-req=ext-xml` to temporarily ignore these required extensions.&quot;,&quot;language&quot;:&quot;Bash&quot;,&quot;runVisible&quot;:false}],&quot;activatedIndex&quot;:0}" uuid="452cc755-a744-4c6f-95a0-d7110616de0a">

Try to install the missing extensions:

Then retry** composer install**

### Run the Project