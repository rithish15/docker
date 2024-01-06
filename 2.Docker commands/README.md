# **Basic Docker Commands**
  
Pull docker image
```docker
docker pull <registry>/<repository>/<image>:<image_tag>
```

Run docker image
```docker
docker run <image>:<image_tag>
```

List running/stopped containers
```docker
#only running containers
docker ps 

#Get running and stopped containers
docker ps -a
```
Commands on image
```docker
#remove an image
docker rmi <image>  

#spin up an container in detached mode  
docker run -d <image>

#Execute a command on the container
docker run -it <image> <command>
```

Commands on container
```docker
#stop a running container
docker stop <containerid>

#removes a stopped container
docker rm <containerid>  

docker attach <containerid>

#command executed in interactive mode  
docker exec -it <containerid> <command>

#Execute a command on the container
docker exec <containerid> <command>
```