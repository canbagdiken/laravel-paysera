# Laravel Paysera
Package that helps to use Paysera API in laravel application.

## Installation
First require package with composer:
```sh
$ composer require canbagdiken/laravel-paysera
```
Then add service provider to config/app.php:
```php
'providers' => [
    ...
    Canbagdiken\Paysera\PayseraServiceProvider::class,
],
```
Facede to aliases:
```php
'aliases' => [
    ...
    'Paysera' => Canbagdiken\Paysera\Facades\Paysera::class,
],
```
And last is to publish config, migrations and view:
```sh
$ php artisan vendor:publish --provider="Canbagdiken\Paysera\PayseraServiceProvider"
```
