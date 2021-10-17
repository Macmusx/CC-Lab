# Build

```docker
docker build -t nodejstest .
```

# Run
```docker
docker container run -p 12345:8080 nodejstest
```

# Stop & Remove
```docker
docker container stop <NAME>
docker container rm <NAME>
```
