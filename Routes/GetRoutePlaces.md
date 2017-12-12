## Method ##

GET

## Route ##

routes/get_route_places/<route_id>

## Headers ##

* Content-type: application/json
* Authorization: token

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
    "lng",
    "lat",
    "google_id",
    "updated_at",
    "created_at",
    "user_id",
    "cover_id"
  },
  ...
]

```   
id, vote_num, cover_id, user_id - integer; score, lat, lng - float; other - strings

* 403 - Forbidden
* 404 - Not found