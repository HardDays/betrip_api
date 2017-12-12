## Method ##

PUT

## Route ##

routes/update/<route_id>

## Headers ##

* Content-type: application/json
* Authorization: token

## Body ##
```
#!json
{
    "name",
    "description",
    "from" : {
      "id"
    },
    "to" : {
      "id"
    },
    "cover" :{
        "base64",
        "filetype"
    }
}
```  

Necessary fields: from, to

OR

```
#!json
{
    "name",
    "description",
    "from" : {
      "address"
    },
    "to" : {
      "address"
    },
    "cover" :{
        "base64",
        "filetype"
    }
}
```   

Necessary fields: from, to


OR
```
#!json
{
    "name",
    "description",
    "from" : {
      "lng",
      "lat"
    },
    "to" : {
      "lng",
      "lat"
    },
    "cover" :{
        "base64",
        "filetype"
    }
}
```
Necessary fields: from, to

from, to - Place objects, see places for addition fields like title or description,
if they given as address or lat/lng, they will be created

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
    "user_id",
    "created_at",
    "updated_at",
    "from_id",
    "to_id",
    "cover_id"
}

```   
id, user_id, vote_num, from_id, to_id, cover_id - integer; score - float; other - strings

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