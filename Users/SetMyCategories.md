## Method ##

POST

## Route ##

users/set_my_categories

## Headers ##

* Content-type: application/json
* Authorization: token

## Body ##

```
#!json
{

     "categories": ["category1", "category2", ...]

}
```   
where category - water, mountains, architecture, rel_building, nature, monument, other

## Return value ##

* 200 - OK


* 403 - Forbidden