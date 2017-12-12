## Method ##

POST

## Route ##

testers/create

## Headers ##

* Content-type: application/json

## Body ##

```
#!json
{
    "email",
    "name",
    "like",
    "text",
    "traveling",
    "types_of_sights"
}

```

Necessary fields: email
All fields are string

## Return value ##

* 201 - Created

```
#!json
{
    "id",
    "email",
    "name",
    "like",
    "text",
    "traveling",
    "types_of_sights"
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