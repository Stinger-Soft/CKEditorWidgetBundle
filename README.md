# CKEditor plugin Widget Bundle for Symfony2
Symfony2 Bundle to integrate the CKEditor plugin Widget

## Current Version

Widget v4.4.8

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "stinger/ckeditor-widget-bundle": "~4.4.8"
    }
}
```

### Add bundle to your application kernel

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Stinger\CKEditorWidgetBundle\StingerCKEditorWidgetBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update stinger/ckeditor-widget-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ php app/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ php app/console assets:install --symlink web
```

### Usage

``` yaml
trsteel_ckeditor:
    external_plugins:
      widget:
        path: 'bundles/stingerckeditorwidget'
```



# Licenses

Refer to the source code of the included files for license information

# References

1. http://ckeditor.com/addon/wdget
2. http://symfony.com
