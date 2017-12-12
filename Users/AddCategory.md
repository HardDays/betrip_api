## Method ##

POST

## Route ##

users/add_my_category

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

Necessary fields: category - name of category, string

## Return value ##

* 200 - OK
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