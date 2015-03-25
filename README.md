Encrypt / Decrypt for PHP

######################
# HOW TO USE IT (PHP)

$mcrypt = new MCrypt();

$mcrypt->setKey($secretKey); // must be 16 bytes
$mcrypt->setIv($secretIv); // must be 16 bytes

/* Encrypt */
$encrypted = $mcrypt->encrypt("Text to encrypt");

/* Decrypt */

$decrypted = $mcrypt->decrypt($encrypted);