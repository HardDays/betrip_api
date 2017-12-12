## Method ##

PUT

## Route ##

users/update/<id>

## Headers ##

* Content-type: application/json
* Authorization: token

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

* 200 - OK

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
id - integer;  other - strings

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