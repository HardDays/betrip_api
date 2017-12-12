## Method ##

POST

## Route ##

users/upload_photo

## Headers ##

* Content-type: application/json
* Authorization: token

## Body ##

```
#!json
{
    "base64"
}

```

Necessary fields: base64

## Return value ##

* 200 - Ok

```
#!json
{
    "id",
    "email",
    "first_name",
    "second_name",
    "last_name",
    "phone",
    "cover_id",
    "updated_at",
    "created_at"
}

```   
id, cover_id - integer, other - strings

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