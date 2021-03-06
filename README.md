# Jiffy Universal Timestamps


[![Author](http://img.shields.io/badge/author-@castarco-blue.svg?style=flat-square)](https://twitter.com/castarco)
[![Build Status](https://img.shields.io/travis/Litipk/php-jiffy/master.svg?style=flat-square)](https://travis-ci.org/Litipk/php-jiffy)
[![Coverage Status](https://img.shields.io/scrutinizer/coverage/g/litipk/php-jiffy.svg?style=flat-square)](https://scrutinizer-ci.com/g/litipk/php-jiffy/code-structure)
[![Quality Score](https://img.shields.io/scrutinizer/g/litipk/php-jiffy.svg?style=flat-square)](https://scrutinizer-ci.com/g/litipk/php-jiffy)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE)
[![Packagist Version](https://img.shields.io/packagist/v/Litipk/php-jiffy.svg?style=flat-square)](https://packagist.org/packages/Litipk/php-jiffy)
[![Total Downloads](https://img.shields.io/packagist/dt/litipk/php-jiffy.svg?style=flat-square)](https://packagist.org/packages/litipk/php-jiffy)


## Installation

```bash
composer require litipk/php-jiffy
```

## Usage

The PHP Jiffy library provides the `UniversalTimestamp` class, which allows you to record timestamps with milliseconds
and microseconds precision and to convert it to other "timestamp types" whenever you need to do it.

The supported PHP versions are **5.5**, **5.6**, **7.0** and **HHVM**.

```php
<?php

use Litipk\Jiffy\UniversalTimestamp;

$now = UniversalTimestamp::now();
$fromDateTime = UniversalTimestamp::fromDateTimeInterface(new \DateTime());
$fromMongoDate = UniversalTimestamp::fromMongoDate(new \MongoDate());
```

**Notice:** The MongoDB related methods are only available when the `mongo` or `mongodb` extensions are loaded.

## Integration with Doctrine
If you want to use Jiffy's UniversalTimesamp objects in your Doctrine models, you can use our adapter layers:

* [**Jiffy Universal Timestamps for MongoDB ODM**](https://github.com/Litipk/doctrine-mongodb-jiffy/)
* **Jiffy Universal Timestamps for Doctrine ORM** : *Work in progress*.
