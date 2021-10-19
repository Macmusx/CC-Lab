# 1. Build image from Dockerfile
```docker
docker build -t api-laborator1-image .
```

# 2. Create bridge network
```docker
docker network create -d bridge laborator1-db-network
```

# 3. Create volume
```docker
docker volume create laborator1-db-persistent-volume
```

# 4. Run in background a container for a db with specs
```docker
docker container run -it -d --name laborator1db --mount source=init-db.sql,target=/docker-entrypoint-initdb.d/init-db.sql  -e POSTGRES_USER=admin -e POSTGRES_PASSWORD=admin -e POSTGRES_DB=books --network=laborator1-db-network -v laborator1-db-persisten-volume:/var/lib/postgresql/data postgres
docker container inspect ${ID} // verify in config file if the specs are fine
````
# 5. Run in background a container for an app with specs and in the same network with the db


