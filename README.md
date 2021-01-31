# go_postgresql_streaming
 Go webserver that streams data to browser from PostgreSQL procedure with a trigger.  

## Prerequisites
Start up a Docker container with a PostreSQL database:
```shell
docker run --name postgres -e POSTGRES_PASSWORD=password -p 5433:5432 -v postgres_data:/var/lib/postgresql/data -d postgres:alpine
```
Check your running database using `docker stats`. If there is a problem, change external port from 5433 to another free port.

### Running the Go server
Start up the server as a Go package by executing in the root: `go run meadium_streaming`
Visit the `http://localhost` to see the server notifications rendered in the browser.
