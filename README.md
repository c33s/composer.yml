# Composer.yml

If you dislike the [JSON][link_json] format of [`composer.json`][link_composer_json], you can alternatively use `composer.yml` and convert the [YAML][link_yaml] file to [JSON][link_json] before every composer run. This can be achieved best by a simple script. 
 
## YAML to JSON converter

### Information
For easier usage of the `composer.yml` this repo provides a precompiled version of [`igorw's`][link_igorw] [`composer-yaml`][link_composer-yaml], which can be used to convert [YAML][link_yaml] to [JSON][link_json] and vice versa. 

### Download
You can download the precompiled [YAML][link_yaml] to [JSON][link_json] converter [`composer-yaml.phar`][link_download] below.

[** download**][link_download]

## Documentation

For documentation, see:

    Resources/doc/

[Read the documentation](Resources/doc/index.md)

## License

This bundle is released under the MIT license. See the complete license in the
bundle:

    Resources/doc/LICENSE

[Read the documentation](Resources/doc/LICENSE)

[link_igorw]:         https://github.com/igorw
[link_composer-yaml]: https://github.com/igorw/composer-yaml
[link_download]:      dist/composer-yaml.phar?raw=true
[link_json]:          https://en.wikipedia.org/wiki/JSON
[link_yaml]:          https://en.wikipedia.org/wiki/YAML
[link_composer_json]: https://getcomposer.org/doc/04-schema.md