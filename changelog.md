# Changelog

## 1.0.1 - November 23, 2026

Added:
* `Backdrop\Tools\Collection` implements `JsonSerializable`, with a `jsonSerialize()` method that returns a JSON-ready array of the collection's items, serializing any item that is itself `JsonSerializable`. Themes no longer need their own `Collection` subclass for this.

## 1.0.0 - November 17, 2026
The first official release of Backdrop Tools. It includes `Backdrop\Tools\Collection`, an `ArrayObject` with `add()`, `get()`, `has()`, `remove()` and `all()` methods, and property access to its items. It is used by `backdrop-dev/view`.

Changed:
* Requires PHP 7.4 or later, like Backdrop 2.0.

Fixed:
* `Collection::get()` and the magic `__get()` return `null` for a missing item instead of raising an "Undefined array key" warning.
