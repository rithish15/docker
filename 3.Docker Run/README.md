# **Docker Run Commands**
  
## Run interactively on pseudo terminal
```docker
docker run -it <image>:<image_tag>
```

## Port mapping
```docker
#maps nodeport to containerport
docker run -p 8080:8000 <image>:<image_tag>
```
## Volume mapping
```docker
#Maps node directory to container to persist data
docker run -v  /opt/datadir:/var/lib/mysql <image>:<image_tag>
```

## Inspect
```docker
#Get detailed information on container
docker inspect <containerid>
```

## logs
```docker
#Get logs of running container
docker logs <containerid>
```