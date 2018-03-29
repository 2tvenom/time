# Time library

Installation
---

Install the latest version with composer, you have to add a [private VCS repository](https://getcomposer.org/doc/05-repositories.md#using-private-repositories) as described below:

```json
{
  "require": {
    "propellerads/time": "*"
  },
  "repositories": [
    {
      "type": "vcs",
      "url":  "git@github.com:propellerads/time.git"
    }
  ]
}
```

Usage
-----
```php
<?php
require_once "vendor/autoload.php";

use PropellerAds\Time\Time;

$nextWeek = time() + Time::WEEK;
echo 'Next week: '. date('Y-m-d', $nextWeek) . PHP_EOL;
```
