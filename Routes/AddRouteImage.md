## Method ##

POST

## Route ##

routes/add_route_image/<route_id>

## Headers ##

* Content-type: application/json
* Authorization: token

## Body ##
```
#!json
{
    "base64",
    "filetype"
}
```  

Necessary fields: base64, filetype

## Return value ##

* 200 - OK

```
#!json
{
    "id",
    "base64",
    "filetype",
    "hashed",
    "created_at",
    "updated_at"
}

```   
id - integer; other - strings

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