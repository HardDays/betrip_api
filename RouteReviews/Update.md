## Method ##

PUT

## Route ##

route_reviews/update/<id>

## Headers ##

* Content-type: application/json
* Authorization: token

## Body ##

```
#!json
{
    "text",
    "score"
}
```  

Necessary fields: score

## Return value ##

* 200 - Ok

```
#!json

{
    "id",
    "user_id",
    "route_id",
    "text",
    "score",
    "updated_at",
    "created_at",
}

```   
id, user_id, route_id - integer; score - float; other - strings

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