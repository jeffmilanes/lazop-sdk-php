# PHP Library for the Lazada Open API
Usage of this library is also available at [Lazada Open API](https://open.lazada.com)

# Requirements
PHP SDK requires PHP 5 or newer version

# Composer Installation

Run the following command:
```bash
composer require jeffmilanes/lazop-sdk-php
```

Usage
-----

Sample Usage
```php
use jeffmilanes\PHPLazadaSDK\LazopClient;
use jeffmilanes\PHPLazadaSDK\LazopRequest;

...
$c = new LazopClient('https://api.lazada.test/rest', '${appKey}', '${appSecret}');
$request = new LazopRequest('/mock/api/get');
$request->addApiParam('api_id',1);
$request->addHttpHeaderParam('cx','test');
    
var_dump($c->execute($request));
...

```
