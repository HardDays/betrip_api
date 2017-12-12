## Method ##

POST

## Route ##

auth/login

## Headers ##

* Content-type: application/json

## Body ##

```
#!json
{
    "email",
    "password"
}

```
## Return value ##

* 200 - OK

```
#!json
{
    "token"
}

```   

* 401 - Unauthorized