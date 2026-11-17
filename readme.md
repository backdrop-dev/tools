# Backdrop\Tools
Backdrop Tools is a collection of helper classes and functions for developing plugins and themes.

## Requirements
* [ClassicPress](https://www.classicpress.net)
* [WordPress](https://wordpress.org)
* [PHP 7.1](https://www.php.net/releases/7_1_33.php)
* [Composer](https://getcomposer.org)

## Collection
`Backdrop\Tools\Collection` is an `ArrayObject` with helper methods. Items can also be read and written as properties.

```php
$collection = new Backdrop\Tools\Collection( [ 'one' => 1 ] );

$collection->add( 'two', 2 );
$collection->three = 3;

$collection->get( 'two' );     // 2
$collection->has( 'three' );   // true
$collection->get( 'missing' ); // null
$collection->remove( 'one' );
$collection->all();            // [ 'two' => 2, 'three' => 3 ]
```

## Copyright and License
This project is license under GNU GPL, version 2 or higher

2019-2026. Benjamin Lu