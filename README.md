# Laravel Simplesheet

🚀 Easy and performant Excel exports and imports in Laravel

[![Latest Version on Packagist](https://img.shields.io/packagist/v/rabiloo/laravel-simplesheet.svg)](https://packagist.org/packages/rabiloo/laravel-simplesheet)
[![GitHub Tests Action Status](https://img.shields.io/github/workflow/status/rabiloo/laravel-simplesheet/Tests?label=tests)](https://github.com/rabiloo/laravel-simplesheet/actions?query=workflow%3ATests+branch%3Amaster)
[![Total Downloads](https://img.shields.io/packagist/dt/rabiloo/laravel-simplesheet.svg)](https://packagist.org/packages/rabiloo/laravel-simplesheet)

![Laravel Simplesheet](https://banners.beyondco.de/Laravel%20Simplesheet.png?theme=light&packageManager=composer+require&packageName=rabiloo%2Flaravel-simplesheet&pattern=brickWall&style=style_1&description=Easy+and+performant+Excel+exports+and+imports+in+Laravel&md=1&showWatermark=0&fontSize=100px&images=view-grid)


## TODO

- [x] Change package name
- [ ] Change namespace
- [ ] Change from box/spout to openspout/openspout
- [ ] Update to openspout/openspout:4.x
- [ ] Update and refactor code and tests
- [ ] Update GitHub workflow
- [x] Update README, LICENSE, CHANGELOG
- [ ] Update documents
- [ ] Release first version

## Rationale

[Laravel Excel](https://laravel-excel.com) is an amazing package and I highly recommend it. One problem I've had with it comes from using [PhpSpreadsheet](https://phpspreadsheet.readthedocs.io/): working with really big datasets requires a lot of memory, even when the exports/imports are chunked. Some of the features provided by PhpSpreadsheet, like cell mapping and formulas, require it to hold entire document represented by objects in memory.

This package use [Openspout](https://github.com/openspout/openspout) (formerly known as Box Spout) to easy and performant Excel exports and imports in Laravel.

## Features

- **Easily export** from different sources: an array, Laravel Collection or query, to different supported formats (CSV, ODS, TSV, XLSX)

- **Supercharged imports** import of workbooks and worksheets to Eloquent models with batch inserts! Have large files? Your entire import can happen in the background. If you like, you can even handle each row youself!

- **Memory efficient.** Using Box Spout allows this package to use considerably less memory than some alternatives.

Compared to Laravel Excel, this package provides less features because it uses a different library for working with spreadsheets under the hood. However it assures that exports and imports are fast and require less memory.

## Installation

You can install the package via composer:

```bash
composer require rabiloo/laravel-simplesheet
```

## Usage

You can find the full documentation of Laravel Simplesheet [on the website](https://rabiloo.github.io/laravel-simplesheet).


## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## Contributing

Please see [CONTRIBUTING](.github/CONTRIBUTING.md) for details.

## Security Vulnerabilities

Please review [our security policy](../../security/policy) on how to report security vulnerabilities.

## Credits

This package uses a lot of code copied from [Laravel Excel](https://laravel-excel.com) and probably wouldn't exist without it, so a big thanks to the Laravel Excel team for their work on that amazing package. Make sure to check it out!

This package was created by [Nenad Živanović](https://github.com/nikazooz). Thanks him so much.

From 2022, after this package had been [abandoned](https://github.com/nikazooz/laravel-simplesheet/commit/83f4f15452ca71ef00cbbe73b731c526d4bcaafd), Oanh Nguyen and his team continue to maintain and develop it.  

- [Nenad Živanović](https://github.com/nikazooz)
- [Oanh Nguyen](https://github.com/oanhnn)
- [All Contributors](../../contributors)

## License

The MIT License (MIT). Please see [License File](LICENSE) for more information.
