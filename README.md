# Oefenweb Code Sniffer for CakePHP 3

This code works with [phpcs](https://github.com/squizlabs/PHP_CodeSniffer) and checks code against the coding standards used at Oefenweb.

## Installation

It's generally recommended to install these code sniffs with `composer`:

```sh
mkdir CakePHP3Oefenweb && cd $_ && composer require oefenweb/cakephp-codesniffer=^3.0.0;
```

```sh
vendor/bin/phpcs \
  --config-set installed_paths "${PWD}/vendor/cakephp/cakephp-codesniffer,${PWD}/vendor/oefenweb/cakephp-codesniffer,${PWD}/vendor/phpcompatibility/php-compatibility" \
;
```

This lets `phpcs` know where to find your new sniffs. Ensure that you do not overwrite any existing `installed_paths` value.

## Usage

```sh
vendor/bin/phpcs --standard=CakePHPOefenweb ~/foo/bar/index.php;
```
