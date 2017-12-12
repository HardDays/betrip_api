## Method ##

POST

## Route ##

auth/login_google

## Headers ##


## Body ##

{

    "authorization_code"

}

google_token - access token from google Oauth2

## Return value ##

* 200 - OK

```
#!json
{
    "token"
}

```   

* 401 - Unauthorized