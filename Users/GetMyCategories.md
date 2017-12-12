## Method ##

GET

## Route ##

users/get_my_categories

## Headers ##

* Content-type: application/json
* Authorization: token

## Body ##

Empty 

## Return value ##

* 200 - OK

```
#!json
["category1", "category2", ...]
```   
where category - water, mountains, architecture, rel_building, nature, monument, other

* 403 - Forbidden