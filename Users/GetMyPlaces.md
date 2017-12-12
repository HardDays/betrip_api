## Method ##

GET

## Route ##

users/get_my_places

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
    "lng",
    "lat",
    "google_id",
    "updated_at",
    "created_at",
    "user_id",
    "address",
    "cover_id"
  },
  ...
]

```   
id, user_id, cover_id, vote_num - integer; lng, lat, score - float; other - strings

* 403 - Forbidden