# Worldpay PHP Library 3.0.0

This is a fork of the [official Worldpay PHP library](https://github.com/Worldpay/worldpay-lib-php),
which is currently unmaintained.

## Installation

### Composer
Add to your composer.json:
```javascript
"jontjs/worldpay-lib-php": "~3.0.0"
```

Or run:
```bash
composer require jontjs/worldpay-lib-php:~3.0.0
```
### Manual

If you need to use this library in a legacy environment without auto-loading, you can
require the `init.php` file as shown below.

```php
require_once('worldpay-php/init.php');
```

## Documentation
https://online.worldpay.com/docs

## API Reference
https://online.worldpay.com/api-reference

## Examples
The examples require editing to support PHP 5.3.

### index.php
Uses WorldpayJS to generate a token that is posted to create_order.php.
**Change your client key**

### create_order.php
Creates a Worldpay order with a posted token.
**Change your service key*

### 3ds_redirect.php
Authorizes a 3DS order
**Change your service key*

### refund.php
Enter your Worldpay order code and posts it to refund_order.php

### refund_order.php
Refunds a Worldpay order with a posted order code
**Change your service key**

### partial_refund.php
Enter your Worldpay order code and amount to refund and posts it to partial_refund_order.php

### partial_refund_order.php
Refunds a Worldpay order with a posted order code
**Change your service key**

### stored_cards.php
Enter your Worldpay reusable token and posts it to stored_cards.php

### get_stored_cards.php
Shows stored card details from posted token
**Change your service key*

## Requirements

PHP 5.3+
Curl
