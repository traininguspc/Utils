

## PostGres Install Commands

```

docker run -p 5432:5432 --name postgresql -e POSTGRES_PASSWORD=password -d -v 'postgresql-volume:/var/lib/postgresql/data' postgres:11

```
