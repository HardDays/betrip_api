## Method ##

GET

## Route ##

places/get_all

## Headers ##

* Content-type: application/json

## Parameters ##

All parameters are optional and used for search and pagination

* user_id
* name
* description
* from_id
* to_id
* limit
* offset

Example: 
```
places/get_all?name=kek&user_id=1&limit=10&offset=0
```
WARNING: name and description searched by LIKE query (case-insensitive, high cost)

## Body ##

Empty

## Return value ##

* 200 - OK

```
#!json
[
  {
    "id",
    "name",
    "score",
    "vote_num",
    "description",
    "user_id",
    "updated_at",
    "created_at",
    "from_id",
    "to_id",
    "cover_id",
    "distance",
    "distance",
    "travel_time",
    "likes_count",
    "reposts_count"
  }
  ...
]
```   
id, user_id, vote_num, from_id, to_id, cover_id, distance, travel_time, likes_count, reposts_count - integer; score - float; other - strings

distance in meters, travel_time in seconds

* 403 - Forbidden