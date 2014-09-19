Simple Yii1 PSR-3 logger proxy
==============================

Installation
------------

Put `YiiPsr3Proxy.php` into components folder.
Include it in config/main.php:
```php
  'components' => array(
     'psr3log' => array(
         'class' => 'application.components.YiiPsr3Proxy'
     ),
  ),

```

Via composer
------------
You really need composer for simple class? ;)

Usage
-----

Use it in any component, that requires PSR-3 logger
```php
   $some->logger = Yii::app()->psr3log;
```