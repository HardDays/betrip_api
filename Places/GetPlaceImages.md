## Method ##

GET

## Route ##

routes/get_place_images/<route_id>

## Headers ##

* Content-type: application/json

## Body ##

Empty

## Return value ##

* 200 - OK

```
#!json
[
  {
    "id",
    "base64",
    "filetype",
    "hashed",
    "created_at",
    "updated_at"
  },
  ...
]

```   

id - integer; other - strings

* 403 - Forbidden
* 404 - Not found