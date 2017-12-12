## Method ##

PUT

## Route ##

places/update/<id>

## Headers ##

* Content-type: application/json
* Authorization: token

## Body ##
```
#!json
{
    "name",
    "description",
    "lng",
    "lat",
    "cover" :{
        "base64",
        "filetype"
    }
}
```   

Necessary fields: lat, lng

OR
```
#!json
{
    "name",
    "description",
    "address",
    "cover" :{
        "base64",
        "filetype"
    }
}
```  

Necessary fields: address

## Return value ##

* 200 - OK

```
#!json
{
    "id",
    "name",
    "score",
    "vote_num",
    "description",
    "lng",
    "lat",
    "google_id",
    "updated_at",
    "created_at",
    "user_id",
    "address", 
    "cover_id"
}

```   

id, user_id, cover_id, vote_num - integer; lat, lng, score - float; other - strings

* 403 - Forbidden
* 404 - Not found
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