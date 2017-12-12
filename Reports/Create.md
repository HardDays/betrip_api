## Method ##

POST

## Route ##

reports/create

## Headers ##

* Content-type: application/json
* Authorization: token

## Body ##

```
#!json
{
    "title",
    "body"
}

```

## Return value ##

* 201 - Created

```
#!json
{
    "id",
    "title",
    "body",
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