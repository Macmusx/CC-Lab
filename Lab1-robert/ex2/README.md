# Build
```docker
docker build -t nodejstest .
```

# Run
```docker
docker container run -it -d -p  12345:8080  nodejstest
```

# Stop & Remove
```docker
docker container stop ${ID}
docker container rm ${ID}
[docker system prune]
```
