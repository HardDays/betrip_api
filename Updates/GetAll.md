## Method ##

GET

## Route ##

updates/get_all

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
    "id": 1,
    "android": "1.0.0-alpha",
    "ios": "0.0.0",
    "web": "0.0.0",
    "created_at": "2017-09-06T10:23:32.635Z",
    "updated_at": "2017-09-06T10:23:32.635Z"
  },
  ...
]

```

id - integer, other - strings

* 403 - Forbidden