## Method ##

GET

## Route ##

routes/get_liked_routes

## Headers ##

* Content-type: application/json
* Authentication: token

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
    "created_at",
    "updated_at",
    "from_id",
    "to_id",
    "cover_id",
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
* 404 - Not found