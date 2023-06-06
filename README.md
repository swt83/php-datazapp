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

## Notes

- ``PhoneScrubAPI`` - requires ``Phone``, delivers ``PhoneType``
- ``EmailVerificationAPI`` - requires ``Email``, delivers ``Status``

The docs are only available for logged-in users with downloadable PDF files.