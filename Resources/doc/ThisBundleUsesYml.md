# composer.yml

_**Attention - The Bundle/Component linked here uses the `composer.yml` format**_

Because json is not a really handy format to read and it also lacks in commenting support, the Bundle/Component linking her uses the `composer.yml` format. 

This means all changes to composer data must be done in `composer.yml` first and afterwards converted to `composer.json` using [`composer-yaml.phar`][link_composer-yaml_phar]. 

## Setup
* Install and setup both [`composer.phar`][link_composer_phar] and [`composer-yaml.phar`][link_composer-yaml_phar].
* Create a script file `composer.sh`, which call [`composer-yaml.phar`][link_composer-yaml_phar] before running composer. 

composer.sh
```
#!/bin/bash
php composer-yaml.phar convert composer.yml composer.json
php composer.phar update
```

## Usage
```
# edit the existing composer.yml and leave the composer.json untouched
php composer-yaml.phar convert composer.yml composer.json
php composer.phar update
```
or use the composer.sh script
```
# edit the existing composer.yml and leave the composer.json untouched
bash composer.sh
```

this Bundle supports the composer.yml format. composer-yaml.phar is used, to convert from yml to json. In this manual all composer code snippets are in yml format. Create a script file, which call the yml to json converter before running composer. Make sure you have both composer and composer-yaml commands at your fingertips.

[link_composer-yaml_phar]: dist/composer-yaml.phar?raw=true
[link_composer_phar]: https://getcomposer.org/download/
