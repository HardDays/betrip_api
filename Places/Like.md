## Method ##

POST

## Route ##

places/like/<place_id>

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
* 404 - Place not found
* 422 - Unprocessable entity