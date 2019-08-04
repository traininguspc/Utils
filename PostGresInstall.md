

## PostGres Install Commands

```Docker

docker run -p 5432:5432 --name postgresql -e POSTGRES_PASSWORD=password -d -v 'postgresql-volume:/var/lib/postgresql/data' postgres:11


docker exec -it postgresql psql -U postgres

 
 docker run -p 8082:80 --name pgAdmin -v "C:/dockerexternalfiles/pgadmin:/var/lib/pgadmin" -e "PGADMIN_DEFAULT_EMAIL=contactusjr@gmail.com" -e "PGADMIN_DEFAULT_PASSWORD=password" -d dpage/pgadmin4

172.17.0.2


```
https://glenmccallum.com/wp-content/uploads/2018/06/docker-container-inspect.png



Open it up in your browser at http://localhost:8080. Since this is run locally for you on your dev machine only you can skip the SSL certifcate and https configuration. However, if you plan on accessing this tool over a network (or the internet) see the notes on the docker hub page for further details.

pgAdmin Welcome Screen

 

By default docker containers run in bridged networking mode. So when you’re connecting from your pgAdmin container to your postgresql container you have to either connect to the host on the mapped port 5432. Or you can connect to the postrgresql container directly on port 5432. Considering the possible-transient nature of the IP address on your host machine I would consider connecting from container to container directly.

Connect to your PostgreSQL instance by right clicking on ‘Servers’ in the left pain, then ‘Create>’, ‘Server…’.

You can get the IP address of the postgresql container by using the inspect command from your host. Then scroll to the bottom and find the ip address.
```
docker inspect postgresql
Docker Inspect Container
```
Then use that IP from the pgAdmin Create Server interface and the password from above when you spun up the postresql container (‘postgres’ is the default username).

pgAdmin To Container Connection

 

To start and stop the pgAdmin container (my equivalent to opening and closing an application) just run:
```
docker start pgAdmin
docker stop pgAdmin
```


## RedMine Install

```
docker volume create redmine-data

```
