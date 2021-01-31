# go_postgresql_streaming
 Go webserver that streams data to browser from PostgreSQL procedure with a trigger.  

## Prerequisites
Start up a Docker container with a PostreSQL database:
```shell
docker run --name postgres -e POSTGRES_PASSWORD=password -p 5433:5432 -v postgres_data:/var/lib/postgresql/data -d postgres:alpine
```
