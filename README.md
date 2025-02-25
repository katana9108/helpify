# A package that catalogs common utility functions for Laravel

[![Latest Version on Packagist](https://img.shields.io/packagist/v/piscarocarlos/helpify.svg?style=flat-square)](https://packagist.org/packages/piscarocarlos/helpify)
[![Total Downloads](https://img.shields.io/packagist/dt/piscarocarlos/helpify.svg?style=flat-square)](https://packagist.org/packages/piscarocarlos/helpify)

This package consolidates a set of commonly used utility functions for Laravel. It aims to streamline development by providing practical and reusable tools for common tasks. Whether it's string manipulation, date handling, or other routine operations, this helper package simplifies developers' lives by centralizing these essential functionalities.

## Support us

We invest a lot of resources into creating [best in class open source packages](https://spatie.be/open-source). You can support us by [buying one of our paid products](https://spatie.be/open-source/support-us).

We highly appreciate you sending us a postcard from your hometown, mentioning which of our package(s) you are using. You'll find our address on [our contact page](https://spatie.be/about-us). We publish all received postcards on [our virtual postcard wall](https://spatie.be/open-source/postcards).

## Installation

You can install the package via composer:

```bash
composer require piscarocarlos/helpify
```

And then, if using Laravel 5, include the service provider within `config/app.php`.

```php
'providers' => [
    Piscarocarlos\Helpify\HelpifyServiceProvider::class,
];
```

And, for convenience, add a facade alias to this same file at the bottom:

```php
'aliases' => [
    'Helpify' => Piscarocarlos\Helpify\Facades\Helpify::class,
];
```

## Usage

```php
use Helpify\Helpers;

$url = 'https://www.example.com';
$shortenedURL = short_url($url);
// OR
$shortenedURL = Helpers::short_url($url);
```

## Testing

```bash
composer test
```

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Security Vulnerabilities

Please review [our security policy](../../security/policy) on how to report security vulnerabilities.

## Credits

- [Carlos Alognon](https://github.com/Piscarocarlos)
- [All Contributors](../../contributors)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
