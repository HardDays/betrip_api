## Method ##

GET

## Route ##

routes/get_route_images/<route_id>

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