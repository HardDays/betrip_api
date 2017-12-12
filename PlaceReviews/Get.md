## Method ##

GET

## Route ##

place_reviews/get/<id>

## Headers ##

* Content-type: application/json
* Authorization: token

## Body ##

Empty  

## Return value ##

* 201 - Ok

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