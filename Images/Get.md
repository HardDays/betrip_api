## Method ##

GET

## Route ##

images/get/<id>

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
    "author_name",
    "author_url",
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