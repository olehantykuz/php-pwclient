## A convenient PayWhirl API wrapper in PHP

The [PayWhirl] PHP library is provided to allow developers to access PayWhirl
services without needing to write their own API wrappers. 

The [Documentation] linked here and below contains all of the available methods 
for interacting with your PayWhirl account. If you would like to see additional 
functionality added, feel free to submit an issue or a pull request.



  [PayWhirl]: https://app.paywhirl.com/
  [PHP]: http://www.php.net/
  [Documentation]: https://api.paywhirl.com/

### Usage Guide

- [Documentation]

## Table of Contents

- [Requirements](#requirements)
- [Installation](#installation)
- [License](#license)
- [About](#about)

## Requirements

- [PHP] 5.6+

## Installation

The recommended way of including this package in your project is by using Composer:

```sh
$ composer require paywhirl/paywhirl
```

Make sure to use Composer's autoload:

```php
require_once __DIR__ . '/vendor/autoload.php';
```

## Usage

To create a new PayWhirl object, you need to pass in your API key and 
secret, which can be found in the [API key section of the main site](https://app.paywhirl.com/api-keys).

```php
use PayWhirl\PayWhirl;

$api_key = "pwpk_xxxxxxxxxxxxxxx";
$api_secret = "pwpsk_xxxxxxxxxxx";

$paywhirl = new \PayWhirl\PayWhirl($api_key, $api_secret);

print_r($paywhirl->getAccount());
```

## License

PayWhirl is copyright © 2016-2018 [PayWhirl Inc.][PayWhirl] This library is free
software, and may be redistributed under the terms specified in the [license].

  [license]: LICENSE.md

## About

[PayWhirl Inc.][PayWhirl] and the names and logos for PayWhirl are
trademarks of PayWhirl inc.

For additional information, please see our [Terms of Use](https://app.paywhirl.com/terms) and [Privacy Policy](https://app.paywhirl.com/privacy)
