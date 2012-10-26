# SimpleBuilder

A Collection of simple builder classes to produce xml and json. Inspired by the [Builder ruby gem](http://rdoc.info/gems/builder) (known from Ruby on Rails).

## Requirements

PHP 5.3

## Installation

Put this lib somewhere and...

### Autoloading

...use [autoloading](http://php.net/manual/en/language.oop5.autoload.php) to load the classes lazily.

```php
spl_autoload_register(function($class) {
		# your loading logic here
});
```

### include/require

...load the classes like in stone age:

```php
include 'SimpleBuilder/lib/JsonBuilder.php'
```

## Usage

```php
$xml = new XmlBuilder;
$xml->foo->bar->baz;
$xml->foo->bla = 'blubb';
$xml->foo->bla['title'] = 'empty';
echo $xml;
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

# License

SimpleBuilder is licensed under the [MIT license](http://opensource.org/licenses/MIT).
