# Jaeger CMS Agnostic Framework

Jaeger allows for cross platform plugin development for various content management and e-commerce systems. Currently, Jaeger supports:

1. [ExpressionEngine (2&3)](https://ellislab.com/expressionengine)
2. [WordPress](https://wordpress.org/)
3. [Craft](https://craftcms.com/)
3. [Concrete5](http://www.concrete5.org/)
4. [PrestaShop](https://www.prestashop.com/)

## Installation 

Add `jaeger-app/jaeger` as a requirement to your `composer.json`:

```bash
$ composer require jaeger-app/jaeger
```

## Philosophy

At the core, Jaeger is a collection of composer libraries that center around a `JaegerApp\Platforms\AbstractPlatform` object. So, while Jaeger does include quite a few libraries for handling things `Db`, `Email`, and such, you're not stuck using any of them outside of the `Plaform` objects. 

It should be noted that Jaeger is best served for your primary business logic and does NOT serve as a replacement for the CMS plugin stub files. You'll still have to create plugins; it's just your internal design that's shared. 

## Todo

Create example multi-platform codebase

## Libraries

### Bootstrap 

[![Build Status](https://travis-ci.org/jaeger-app/bootstrap.svg?branch=master)](https://travis-ci.org/jaeger-app/bootstrap)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/bootstrap/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/bootstrap/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE)

A pre-configured dependency injection container and start-up initialization object. Jaeger Bootstrap will prepare the most common Jaeger objects and make them ready for use as well as function as a stand alone dependency injection container utilizing [Pimple\Container](https://packagist.org/packages/pimple/pimple).

### Compress

[![Build Status](https://travis-ci.org/jaeger-app/compress.svg?branch=master)](https://travis-ci.org/jaeger-app/compress)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/compress/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/compress/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE)

A compression wrapper to manipulate Zip files with PHP using a simple interface. You can create and modify zip archives as well as extract them.

### Console

[![Build Status](https://travis-ci.org/jaeger-app/console.svg?branch=master)](https://travis-ci.org/jaeger-app/console)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/console/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/console/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE)

Handles outputting/writing data to the console. when Jaeger plugins are ran through the Console / Command Line / Shell. 

### DateTime

[![Build Status](https://travis-ci.org/jaeger-app/date-time.svg?branch=master)](https://travis-ci.org/jaeger-app/console)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/date-time/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/console/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

A Trait for handling dates and times without killing yourself.

### Db

[![Build Status](https://travis-ci.org/jaeger-app/db.svg?branch=master)](https://travis-ci.org/jaeger-app/db)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/db/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/db/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

A simple database wrapper that can use either MySQLi or PDO.

### Di

[![Build Status](https://travis-ci.org/jaeger-app/di.svg?branch=master)](https://travis-ci.org/jaeger-app/di)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/di/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/di/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE)

A simple dependency injection container for use with Jaeger (or stand alone). 

### Email 

[![Build Status](https://travis-ci.org/jaeger-app/email.svg?branch=master)](https://travis-ci.org/jaeger-app/email)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/email/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/email/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

`JaegerApp\Email` is an email abstraction that works with both SwiftMailer 3 and 5 (depending on which is already available). Note that the Email object does NOT include any version of SwiftMailer and relies on the host system to provide one. 

### Encrypt

[![Build Status](https://travis-ci.org/jaeger-app/encrypt.svg?branch=master)](https://travis-ci.org/jaeger-app/encrypt)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/encrypt/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/encrypt/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

Provides a simple API to handle encrypting and decrypting strings.

### Errors

[![Build Status](https://travis-ci.org/jaeger-app/errors.svg?branch=master)](https://travis-ci.org/jaeger-app/errors)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/errors/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/errors/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

A base error collection to allow for individual inspections and system validations.

### Exceptions 

[![Build Status](https://travis-ci.org/jaeger-app/exceptions.svg?branch=master)](https://travis-ci.org/jaeger-app/exceptions)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/exceptions/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/exceptions/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

A simple exception handler.

### Files

[![Build Status](https://travis-ci.org/jaeger-app/files.svg?branch=master)](https://travis-ci.org/jaeger-app/files)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/files/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/files/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/files/master/LICENSE)

A simple file handling object.

### Language

[![Build Status](https://travis-ci.org/jaeger-app/language.svg?branch=master)](https://travis-ci.org/jaeger-app/language)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/language/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/language/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

A simple language abstraction to simply keep copy out of your code. This is NOT a translation library.

### Log

[![Build Status](https://travis-ci.org/jaeger-app/log.svg?branch=master)](https://travis-ci.org/jaeger-app/log)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/log/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/log/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

A logging trait.

### Platforms

[![Build Status](https://travis-ci.org/jaeger-app/platforms.svg?branch=master)](https://travis-ci.org/jaeger-app/platforms)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/platforms/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/platforms/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

A CMS Platform abstraction layer for platform agnostic development.

### Regex

[![Build Status](https://travis-ci.org/jaeger-app/regex.svg?branch=master)](https://travis-ci.org/jaeger-app/regex)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/regex/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/regex/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

A simple Regular Expression wrapper.

### Remote

[![Build Status](https://travis-ci.org/jaeger-app/remote.svg?branch=master)](https://travis-ci.org/jaeger-app/remote)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/remote/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/remote/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

A remote file system wrapper around Flysystem.

### Rest Server

[![Build Status](https://travis-ci.org/jaeger-app/rest-server.svg?branch=master)](https://travis-ci.org/jaeger-app/rest-server)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/rest-server/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/rest-server/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

A rest server abstraction to add REST capabilities to a Jaeger based app.

### Rest Client

[![Build Status](https://travis-ci.org/jaeger-app/rest-client.svg?branch=master)](https://travis-ci.org/jaeger-app/rest-client)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/rest-client/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/rest-client/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

A simple REST client to interact with Jaeger REST API installations.

### Settings

[![Build Status](https://travis-ci.org/jaeger-app/settings.svg?branch=master)](https://travis-ci.org/jaeger-app/settings)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/settings/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/settings/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

A settings abstraction.

### Shell

[![Build Status](https://travis-ci.org/jaeger-app/shell.svg?branch=master)](https://travis-ci.org/jaeger-app/shell)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/shell/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/shell/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

A simple shell library to execute commands on the Console. 

### Validate

[![Build Status](https://travis-ci.org/jaeger-app/validate.svg?branch=master)](https://travis-ci.org/jaeger-app/validate)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/validate/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/validate/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

A validation library.

### View

[![Build Status](https://travis-ci.org/jaeger-app/view.svg?branch=master)](https://travis-ci.org/jaeger-app/view)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/jaeger-app/view/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/jaeger-app/view/?branch=master)
[![Author](http://img.shields.io/badge/author-@mithra62-blue.svg?style=flat-square)](https://twitter.com/mithra62)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/jaeger-app/bootstrap/master/LICENSE) 

A view layer for Jaeger based plugins and modules.