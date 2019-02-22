# FP
Functional programming library for PHP

## Features
- Functions are composable: can be partially applied by returning fewer arguments than the arity
- Functions are lazy: operating on traversable structures will always return a Generator
- Functions are namespaced: prevents leakage into global scope

## Installation
Install with composer
```
composer install denheck/fp
```
## Usage
```php
use function denheck\fp\map;
use function denheck\fp\id;

$idMapper = map("id");
$idMapper([1, 2, 3]) === [1, 2, 3];
```
