## Method ##

POST

## Route ##

auth/login_twitter

## Headers ##


## Body ##

{

    "access_token"
    "access_token_secret"

}

access_token, access_token_secret - access tokens from twitter Oauth

## Return value ##

* 200 - OK

```
#!json
{
    "token"
}

```   

* 401 - Unauthorized