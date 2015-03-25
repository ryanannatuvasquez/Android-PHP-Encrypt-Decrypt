Encrypt / Decrypt for PHP

######################
# Installation
{
    "require": {
        "ryanannatuvasquez/android-php-encrypt-decrypt": "dev-master"
    }
}

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
