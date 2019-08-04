

## PostGres Install Commands

```Docker

docker run -p 5432:5432 --name postgresql -e POSTGRES_PASSWORD=password -d -v 'postgresql-volume:/var/lib/postgresql/data' postgres:11


docker exec -it postgresql psql -U postgres

 
 docker run -p 8082:80 --name pgAdmin -v "C:/dockerexternalfiles/pgadmin:/var/lib/pgadmin" -e "PGADMIN_DEFAULT_EMAIL=contactusjr@gmail.com" -e "PGADMIN_DEFAULT_PASSWORD=password" -d dpage/pgadmin4

172.17.0.2


```
https://glenmccallum.com/wp-content/uploads/2018/06/docker-container-inspect.png
