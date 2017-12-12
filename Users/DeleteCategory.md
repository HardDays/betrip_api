## Method ##

DELETE

## Route ##

users/delete_my_category

## Headers ##

* Content-type: application/json
* Authorization: token

## Body ##
```
#!json
{
    "category"
}
```  
where category - water, mountains, architecture, rel_building, nature, monument, other

## Return value ##

* 204 - OK, no content
* 403 - Forbidden