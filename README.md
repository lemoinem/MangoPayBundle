Getting Started With WeMakCustom MangoPayBundle
==============

A bundle to wrappe and simplify the use of Mango Pay 2 Api.

Use this bundle at your own risk.

## Prerequisites

    Symfony 2.3+
    Php 4.4+

## Installation

Installation is a quick 3 step process:

1. Download MangoPayBundle using composer
2. Enable the Bundle
3. Configure your config.yml

### Step 1: Download MangoPayBundle using composer

Add MangoPayBundle in your composer.json:

```js
{
    "require": {
        "wemakecustom/mango-pay-bundle": "dev-master"
    }
}
```

Now tell composer to download the bundle by running the command:

``` bash
$ php composer.phar update wemakecustom/mango-pay-bundle
```

### Step 2: Enable the bundle

Enable the bundle in the kernel:

``` php
<?php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new WMC\MangoPayBundle\WMCMangoPayBundle(),
    );
}
```

### Step 3: Configure your config.yml

``` yaml
# app/config/config.yml

wmc_mongo_pay:

```