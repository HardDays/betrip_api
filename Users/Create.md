## Method ##

POST

## Route ##

users/create

## Headers ##

* Content-type: application/json

## Body ##

```
#!json
{
    "email",
    "password",
    "first_name",
    "second_name",
    "last_name",
    "phone"
}

```

Necessary fields: email, password

## Return value ##

* 201 - Created

```
#!json
{
    "id",
    "email",
    "first_name",
    "second_name",
    "last_name",
    "phone",
    "updated_at",
    "created_at"
}

```   
id - integer, other - strings

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