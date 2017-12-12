## Method ##

GET

## Route ##

routes/get_interesting_places

## Headers ##

* Content-type: application/json

## Params ##

* from - address OR lat,lng

* to - address OR lat,lng

* categories - array of categories, could be: water, mountains, architecture, rel_building, nature, monument, other

Example: categories[]=water&categories[]=nature

Necessary params: from, to

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
    "foursquare_id",
    "updated_at",
    "created_at",
    "user_id",
    "address",
    "cover_id",
    "likes_count",
     "reposts_count"
  },
  ...
]

```   
id, user_id, vote_num, cover_id - integer; score - float; other - strings

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