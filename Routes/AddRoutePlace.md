## Method ##

POST

## Route ##

routes/add_route_place/<route_id>

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

OR
```
#!json
{
    "id"
}
```  

Necessary fields: id - id of existing place

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
id, vote_num, user_id, cover_id - integer; score, lat, lng - float; other - strings

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