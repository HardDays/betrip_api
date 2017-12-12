## Method ##

GET

## Route ##

places/get_places_categories/<place_id>

## Headers ##

* Content-type: application/json
* Authorization: token

## Body ##

Empty 

## Return value ##

* 200 - OK

```
#!json
[
     {
        "id",
        "name",
        "created_at",
        "updated_at"
     },
     ...
]
```   
id - integer; other - strings

* 403 - Forbidden
* 404 - Not found