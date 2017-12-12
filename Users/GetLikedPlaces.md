## Method ##

GET

## Route ##

users/get_liked_places

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
    "lng",
    "lat",
    "google_id",
    "updated_at",
    "created_at",
    "user_id",
    "address",
    "cover_id",
    "likes_count",
    "reposts_count", 
    "categories"
  }
  ...
]
```   
id, user_id, cover_id, vote_num, likes_count, reposts_count - integer; lat, lng, score - float; other - strings; categories - array of strings

* 403 - Forbidden
* 404 - Not found