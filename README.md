Raven Bundle for Symfony2
=======================

## Current Version

Raven.js 3.7.0

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "alexandermatveev/raven-bundle": "*"
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
        new AlexanderMatveev\RavenBundle\AlexanderMatveevRavenBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update alexandermatveev/raven-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ bin/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ bin/console assets:install --symlink web
```

## Usage

Refer to the desired files in your HTML template, e.g.

``` html
<script type="text/javascript" src="{{ asset('bundles/alexandermatveevraven/raven.min.js') }}"></script>
```

## Licenses

Refer to the source code of the included files for license information

## References

1. https://github.com/getsentry/raven-js