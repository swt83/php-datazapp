# DataZapp

A PHP package for working w/ the DataZapp API.

## Install

Normal install via Composer.

## Usage

```php
use Travis\DataZapp;

$test = DataZapp::run($apikey, 'EmailVerificationAPI', [
    ['Email' => '<EMAILADDRESS>',],
]);

$test = DataZapp::run($apikey, 'PhoneScrubAPI', [
    ['Phone' => '<PHONENUMBER>',],
]);
```

See the [documentation](https://usebasin.com/docs/api) for more information.

## Notes

- ``PhoneScrubAPI`` - requires ``Phone``, delivers ``PhoneType``
- ``EmailVerificationAPI`` - requires ``Email``, delivers ``Status``