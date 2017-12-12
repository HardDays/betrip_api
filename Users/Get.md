## Method ##

GET

## Route ##

users/get/<id>

## Headers ##

* Content-type: application/json
* Authorization: token

## Body ##

Empty

## Return value ##

* 200 - OK

If authorized as admin

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

Regular user

```
#!json
{
    "id",
    "cover_id",
    "first_name",
    "last_name",
}

```

* 403 - Forbidden
* 404 - Not found