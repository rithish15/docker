# **Docker Engine**
  
## Docker Engine Architecture
![alt text](../6.Docker-engine/images/docker-engine-arch.png)

## Containerization
Is acheieved by isolating the follwing
  * Namespaces
    * PID
    * Network              
    * Mount process
    * Unix timesharing
    * InterProcess  

## Resources
![alt text](../6.Docker-engine/images/cgroups.png)

## Docker Filesystem
  * /var/lib/docker
    * aufs (storage driver)
    * containers
    * image
    * volumes (default volume location)

## Container Layer
![alt text](../6.Docker-engine/images/container-layer.png)


![alt text](../6.Docker-engine/images/copy-on-write.png)

## Volumes
![alt text](../6.Docker-engine/images/volumes.png)

```docker
#Create volume
docker volume create <volume_name>

#Volume mapping
docker run --mount type=bind,source=<volume_name>,target=/var/lib/mysql mysql
```