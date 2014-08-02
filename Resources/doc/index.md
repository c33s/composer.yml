# composer.yml
* [Why using a different format?](#why-using-a-different-format)
* [YAML to JSON converter](#yaml-to-json-converter)
  * [Information](#information)
  * [Download](#download)
* [Usage](#usage)
  * If composer.yml does not exists (and composer.json does)
  * If composer.yml exists (and composer.json does not)
* Build the composer-yaml.phar file yourself
  * Clone This project
  * Get box.phar
  * Run the build process


## Why using a different format
_Why should you use composer.yml instead composer.json?_

Because json is not a really handy format to read and it also lacks in commenting support.
 
## YAML to JSON converter

### Information
For easier usage of the `composer.yml` this repo provides a precompiled version of [`igorw's`][link_igorw] [`composer-yaml`][link_composer-yaml], which can be used to convert [YAML][link_yaml] to [JSON][link_json] and vice versa. 

### Download
You can download the precompiled [YAML][link_yaml] to [JSON][link_json] converter [`composer-yaml.phar`][link_download] below.

[**download**][link_download]

## Usage
### If composer.yml does not exists (and composer.json does)
```
# create a composer.json file as you are used to it
touch composer.yml
php composer-yaml.phar convert composer.json composer.yml
# edit the composer.yml, you also can use comments.
php composer-yaml.phar convert composer.yml composer.json
```

### If composer.yml exists (and composer.json does not)
```
(touch composer.json)
# edit the composer.yml, you also can use comments.
php composer-yaml.phar convert composer.yml composer.json
```



## Build the composer-yaml.phar file yourself
### Clone This project
```
	git clone https://github.com/c33s/composer.yml.git
```
### Get box.phar
```
    curl -LSs http://box-project.org/installer.php | php  
```
### Run the build process
In the directory where you cloned this project run box.phar (box.json.dist is located in this directory) 
```
	php box.phar build
```

[link_igorw]:         https://github.com/igorw
[link_composer-yaml]: https://github.com/igorw/composer-yaml
[link_download]:      dist/composer-yaml.phar?raw=true
[link_json]:          https://en.wikipedia.org/wiki/JSON
[link_yaml]:          https://en.wikipedia.org/wiki/YAML
[link_composer_json]: https://getcomposer.org/doc/04-schema.md