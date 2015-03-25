Encrypt / Decrypt for PHP

Attention!
==========

This was forked from [serpro/Android-PHP-Encrypt-Decrypt](https://github.com/serpro/Android-PHP-Encrypt-Decrypt). 

### What's New?
- Install using composer
- Setter for `KEY` and `IV`

######################
# Installation
```json
{
    "require": {
        "ryanannatuvasquez/android-php-encrypt-decrypt": "dev-master"
    }
}
```

######################
# Example

```php
$mcrypt = new MCrypt();

$mcrypt->setKey($secretKey); // must be 16 bytes
$mcrypt->setIv($secretIv); // must be 16 bytes

/* Encrypt */
$encrypted = $mcrypt->encrypt("Text to encrypt");

/* Decrypt */

$decrypted = $mcrypt->decrypt($encrypted);
```
