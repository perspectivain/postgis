Postgis
=======
A Yii2 library to convert postgis coordinates to array and array to postgis text

Currently support Point and Polygon types.

Usage
=======
Extend your AR model to postgis AR and use your methods

```
<?php
use perspectivain\yii2-postgis\ActiveRecord as PostgisActiveRecord;

class Customer extends PostgisActiveRecord {
  ...
}

...

$coordinates = $model->postgisToArray('Polygon', 'city_coordinates');

$model->city_coordinates = $model->arrayToPostgis('Polygon', $coordinates);
```

Installing
======
Via composer

```
{
  "require": {
    "perspectivain/yii2-postgis": "*"
  }
}
```
