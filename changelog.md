## 2.1.0 (2024-03-12)
* Add minimum-stability property
* Remove no longer required methods and add PHP type hints
* Update Readme file

## 2.0.1 (2024-03-11)
* Fix Regex to support Enums with Hyphen

## 2.0.0 (2023-05-12)
* Minimum PHP version is now 7.4
* Added hints for latest Propel 2 release

## 1.1.0 (2018-08-21)

* PHP 7.2 compatibility
* Propel's internal now believe that a RealEnum column is of type `VARCHAR`
* It is no longer necessary to set the `phpType` to `string` in the schema
* `convertValueForColumn` method is only added to query classes when an `ENUM` column is detected
* Added this changelog

## 1.0.3 (2018-06-14)

* Whitespace in values of the `valueSet` are now correctly replaced by underscores when generating the constants names. closes [#1](https://github.com/Effenti/propel-real-enum-behavior/issues/1)

## 1.0.2 (2018-04-16)

* Initial public release of the library
