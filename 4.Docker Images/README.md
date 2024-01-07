# **Docker Images**
  
## Creating our own image - Dockerfile
![alt text](../4.Docker%20Images/images/dockerfile.png)

## Layered Architecture
![alt text](../4.Docker%20Images/images/build-layers.png)

```docker
#Use history to get build details
docker history <image>:<image_tag>
```

## Env Variables
```docker
#Pass variables to container
docker run -e <ENV_VARIABLE>=<VALUE> <image>:<image_tag>
```

## Inspect
```docker
#Get env varibles associated with an container
docker inspect <containerid>
```
## CMD vs Entrypoint
Entrypoint : startup command  
CMD : command line arguments (Can be overriden while running the container)
```
Note : Both should be array
```
![alt text](../4.Docker%20Images/images/entrypoint-vs-cmd.png)

