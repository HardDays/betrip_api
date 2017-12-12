## Method ##

POST

## Route ##

places/create

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
    },
    "categories" : [
           {
              "id"
           },
           ...
     ]
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
    },
    "categories" : [
           {
              "id"
           },
           ...
     ]
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