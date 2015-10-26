# Jiffy Universal Timestamps


[![Author](http://img.shields.io/badge/author-@castarco-blue.svg?style=flat-square)](https://twitter.com/castarco)
[![Build Status](https://img.shields.io/travis/Litipk/jiffy/master.svg?style=flat-square)](https://travis-ci.org/jiffy)
[![Coverage Status](https://img.shields.io/scrutinizer/coverage/g/litipk/jiffy.svg?style=flat-square)](https://scrutinizer-ci.com/g/litipk/jiffy/code-structure)
[![Quality Score](https://img.shields.io/scrutinizer/g/litipk/jiffy.svg?style=flat-square)](https://scrutinizer-ci.com/g/litipk/jiffy)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE)
[![Packagist Version](https://img.shields.io/packagist/v/litipk/jiffy.svg?style=flat-square)](https://packagist.org/packages/litipk/jiffy)
[![Total Downloads](https://img.shields.io/packagist/dt/litipk/jiffy.svg?style=flat-square)](https://packagist.org/packages/litipk/jiffy)


## Installation

```bash
composer require litipk/jiffy
```

## Usage

The PHP Jiffy library provides the `UniversalTimestamp` class, which allows you to record timestamps with milliseconds and microseconds precision and to convert it to other "timestamp types" whenever you need to do it.

```php
<?php

use Litipk\Jiffy\UniversalTimestamp;

$now = UniversalTimestamp::now();
$fromDateTime = UniversalTimestamp::fromDateTimeInterface(new \DateTime());
$fromMongoDate = UniversalTimestamp::fromMongoDate(new \MongoDate());
```
