# Jaeger CMS Agnostic Framework

Jaeger allows for cross platform plugin development for various content management and e-commerce systems. Currently, Jaeger supports:

1. ExpressionEngine (2&3)
2. WordPress
3. Concrete5
4. PrestaShop
5. Magento
6. Craft

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

