## Method ##

GET

## Route ##

route_reviews/get_all

## Headers ##

* Content-type: application/json
* Authorization: token

## Parameters ##

All parameters are optional and used for search and pagination

* user_id
* route_id
* limit
* offset

Example: 
```
route_reviews/get_all?user_id=1&route_id=2&limit=10&offset=0
```

## Body ##

Empty

## Return value ##

* 200 - OK

```
#!json
[
  {
    "id",
    "user_id",
    "route_id",
    "text",
    "score",
    "updated_at",
    "created_at",
  },
  ...
]

```   
id, user_id, route_id - integer; score - float; other - strings

* 403 - Forbidden