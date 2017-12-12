## Method ##

POST

## Route ##

places/add_place_category/<place_id>

## Headers ##

* Content-type: application/json
* Authorization: token

## Body ##
```
#!json
{
    "id"
}
```  

Necessary fields: id - id of category

## Return value ##

* 200 - OK

```
#!json
{
        "id",
        "name",
        "created_at",
        "updated_at"
}
```   
id - integer;  other - strings

* 403 - Forbidden
* 422 - Unprocessable entity
```
#!json

{
    "field_name": [
      "error1",
      ...
    ]
}
```