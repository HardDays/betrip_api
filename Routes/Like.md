## Method ##

POST

## Route ##

routes/like/<route_id>

## Headers ##

* Content-type: application/json
* Authorization: token

## Description ##

Create or remove like

## Body ##
EMPTY

## Return value ##

* 204 - OK
* 403 - Forbidden
* 404 - Route not found
* 422 - Unprocessable entity