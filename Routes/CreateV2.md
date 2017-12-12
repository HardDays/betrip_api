## Method ##

POST

## Route ##

routes/create_v2

## Headers ##

* Content-type: application/json

## Body ##
```
#!json
{
    "name",
    "description",
    "from" : place_obj,
    "to" : place_obj,
    "places" :[ 
         place_id1,  place_id2, ...
    ]
}
```  

Necessary fields: from, to

from, to - Place objects, see places for addition fields like title or description,
if they given as address or lat/lng, they will be created, necessary

places - array of places (промежуточные точки кароч), optional

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
    "reposts_count",
    "places": [
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
           "created_at",
           "updated_at",
           "user_id",
           "address",
           "cover_id",
           "likes_count",
           "reposts_count",
           "categories"
       }, 
       ...
    ]
  },
  ...
]

```   
id, user_id, vote_num, from_id, to_id, cover_id, distance, travel_time, likes_count, reposts_count - integer; score - float; categories - array of strings; other - strings

distance in meters, travel_time in seconds

place_obj is
```
#!json
{
      "address"
}
```   
OR
```
#!json
{
      "lng",
      "lat"
}
```



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