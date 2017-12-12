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
* limit
* offset

Example: 
```
places/get_all?name=kek&limit=10&offset=0
```
WARNING: name and description searched by LIKE query (case-insensitive, high cost)

* lng
* lat
* radius

OR

* address
* radius

Used to find near places in radius (km)

Example:
```
places/get_all?name=kek&limit=10&offset=0?lng=0.333&lat=0.222&radius=20
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
id, user_id, cover_id, vote_num - integer; lat, lng, score - float; other - strings


* 403 - Forbidden