# python-web-api-flask-mysql-raw-sql-pop

## Description
Creates an api of `pop` by using raw sql for a flask project.
Has the ability to query by parameters.
If path is not found, will default to 404 error.

Remotely tested with *testify*.

## Tech stack
- python
  - flask
  - sqlalchemy
  - testify
  - requests

## Docker stack
- python:latest
- mariadb:latest

## To run
`sudo ./install.sh -u`
- Get all pops: http://localhost/pop
  - Schema id, breed, and color
- CRUD opperations
  - Create: curl -i -X PUT localhost/pop/<id>
  - Read: http://localhost/pop/<id>
  - Update: curl -i -X POST localhost/pop/<id>/<breed>/<color>
  - Delete: curl -i -X DELETE localhost/pop/<id>

## To stop
`sudo ./install.sh -d`

## For help
`sudo ./install.sh -h`
