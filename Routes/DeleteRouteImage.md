## Method ##

DELETE

## Route ##

routes/delete_route_image/<route_id>

## Headers ##

* Content-type: application/json
* Authorization: token

## Body ##


```
#!json

{
    "id"
}
```
id - place id

## Return value ##

* 204 - Ok, no content
* 403 - Forbidden
* 404 - Not found