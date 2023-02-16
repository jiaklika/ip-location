# ip-location fo php

*Give IP address and return detailed geographic location information*

## Installation

You can install the package via composer:

```bash
composer require jiaklika/ip-location
```

## Quick Start
```php
<?php

require __DIR__ . '/vendor/autoload.php';

$IpLocation = new IpLocation();
$iplocation = $IpLocation->getlocation("you ip address");
//print_r($iplocation);
$area = iconv('GB2312','UTF-8', $iplocation['country'].$iplocation['area']);
```