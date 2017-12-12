## Method ##

GET

## Route ##

usrers/get_my_routes

## Headers ##

* Content-type: application/json
* Authorization: token

## Parameters ##

All parameters are optional and used for search and pagination

* limit
* offset

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
    "travel_time",
    "likes_count",
    "reposts_count",
    "traveled_at"
  },
  ...
]

```   
id, from_id, to_id, vote_num, distance, travel_time, likes_count, reposts_count - integer; score - float; other - strings
traveled_at - datetime string
* 403 - Forbidden