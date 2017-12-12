## Method ##

GET

## Route ##

place_reviews/get_all

## Headers ##

* Content-type: application/json
* Authorization: token

## Parameters ##

All parameters are optional and used for search and pagination

* user_id
* place_id
* limit
* offset

Example: 
```
place_reviews/get_all?user_id=1&place_id=2&limit=10&offset=0
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
    "place_id",
    "text",
    "score",
    "updated_at",
    "created_at",
  },
  ...
]

```   
id, user_id, place_id - integer; score - float; other - strings

* 403 - Forbidden