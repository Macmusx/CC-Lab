# Build
```docker
docker build -t busybox-demo .
```

# Run
```docker
docker run busybox-demo
```
# Interactive run
```docker
docker container run -it busybox-demo wget google.com
```

# Detached
```docker
docker run -it -d busybox-demo id
```