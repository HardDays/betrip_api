## Method ##

GET

## Route ##

users/get_all

## Headers ##

* Content-type: application/json
* Authorization: token

## Parameters ##

All parameters are optional and used for search and pagination

* email
* phone
* first_name
* second_name
* last_name
* limit
* offset

Example:
```
users/get_all/?email=kek@cheburek&limit=10&offset=10
```   
## Body ##

Empty

## Return value ##

* 200 - OK

If authorized as admin

```
#!json
[
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
  },
  ...
]

```   

Regular user

```
#!json
[
  {
    "id",
    "cover_id",
    "first_name",
    "last_name",
  },
  ...
]

```

id, cover_id - integer, other - strings

* 403 - Forbidden