## Method ##

POST

## Route ##

place_reviews/create

## Headers ##

* Content-type: application/json
* Authorization: token

## Body ##

```
#!json
{
    "place_id",
    "text",
    "score"
}

```  

Necessary fields: place_id, score (float)

## Return value ##

* 201 - Created

```
#!json

{
    "id",
    "user_id",
    "place_id",
    "text",
    "score",
    "updated_at",
    "created_at",
}

```   

id, user_id, place_id - integer; score - float; other - strings


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