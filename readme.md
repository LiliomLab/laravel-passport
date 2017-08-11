<p align="center"><img src="https://laravel.com/assets/img/components/logo-passport.svg"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/passport"><img src="https://travis-ci.org/laravel/passport.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/passport"><img src="https://poser.pugx.org/laravel/passport/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/passport"><img src="https://poser.pugx.org/laravel/passport/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/passport"><img src="https://poser.pugx.org/laravel/passport/license.svg" alt="License"></a>
</p>

## Introduction

Laravel Passport is an OAuth2 server and API authentication package that is simple and enjoyable to use.

## Installation

    composer require liliom/passport

## Custom Database Connection

By default, Passport will use the default connection name, but now you can use custom database connection for Passport by adding your connection name in `config/auth.php` (guards.api.connection)

```php
....

'guards' => [
    ...

    'api' => [
        'driver' => 'passport',
        'provider' => 'users',
        'connection' => env('PASSPORT_CONNECTION'),
    ],
],

...
```

## Official Documentation

Documentation for Passport can be found on the [Laravel website](http://laravel.com/docs/master/passport).

## License

Laravel Passport is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT).
