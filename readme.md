# Propel Real Enum Behavior

[![Latest Stable Version](https://poser.pugx.org/antiloopgmbh/propel-real-enum-behavior/v/stable)](https://packagist.org/packages/antiloopgmbh/propel-real-enum-behavior)
[![Total Downloads](https://poser.pugx.org/antiloopgmbh/propel-real-enum-behavior/downloads)](https://packagist.org/packages/antiloopgmbh/propel-real-enum-behavior)
[![License](https://poser.pugx.org/antiloopgmbh/propel-real-enum-behavior/license)](https://packagist.org/packages/antiloopgmbh/propel-real-enum-behavior)

## Requirements

This Behavior was developed for **Propel 2**.  
It was also only tested for **MariaDb** databases for Spryker Webshops.

## Installation

```bash
composer require antiloopgmbh/propel-real-enum-behavior
```

#### schema.xml
Add the behavior either to the root of your database or on the target table.   
Here are two examples:

```XML
<database ...>
    <!-- This will add the real-enum behavior for all enums in the database -->
    <behavior name="real-enum"/>
    <table name="my_table">        
        <column name="my_enum" type="ENUM" valueSet="FIRST,SECOND,THIRD" />
    </table>
</database>
```

```XML
<database ...>
    <table name="my_table">
        <!-- This will add the real-enum behavior for all enums in the table -->
        <behavior name="real-enum"/>
        <column name="my_enum" type="ENUM" valueSet="FIRST,SECOND,THIRD" />
    </table>
</database>
```

#### Usage

This behavior does one thing to make usage of `ENUMS` easier : 

- You will now see the ENUM value from the `valueSet` in the database instead of a number.
