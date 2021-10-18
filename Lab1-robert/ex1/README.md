##### Note: ${x} - placeholder to x 

# 1.Pull
```docker
docker image pull busybox
```

# 2.Run container with command
```docker
docker images //check image
docker container run busybox uptime //run container with uptime inside and graceful close
```
# 3.Interactive run and command
```docker
docker container run -it busybox //run interactive a container
wget google.com// run wget inside
ls // check index.html exists
```

# 4.Run a detached container, attach to it, and run command
```docker
docker container run -it -d busybox // get ID of container
docker container attach ${ID} // attach to it
id
exit

```

# 5.Clean (delete containers/ images)
```docker
docker system prune// clean unnecesarry space
docker container ls//get IDs of running containers
docker stop ${ID}// iterative for all active container built on busybox
docker images // active images
docker rmi busybox// remove busybox
```




