```
sudo apt update
```

```
sudo apt-get install docker.io -y
```
to install docker

```
docker version
```
to check version

```
docker info
```

```
docker help
```

```
sudo apt-get install docker-compose-v2 -y
```
to install docker compose file

```
docker ps
docker ps -a
```
to check containers

```
docker images
```
to list images

```
docker rmi <image-id>
docekr images -aq $(docker rmi )
```
to delete images


```
docker logs <container-id>
```
to check logs

```
vi Dockerfile
```
to create dockerfile

```
docker build -t <image-name> <path-dockerfile>
```
to build an image from dockerfile

```
docker run -d -p <host-port-no>:<container-port-no> <docker-image-name>
```
to run a container from a docker image

```
docker start <conatiner-id>
```
to start container

```
docker stop <conatiner-id>
```
to stop container

```
docker kill <container>
```
to stop container forcefully

```
docker rm <container-name/ container-id>
```
to delete container

```
docker pull <image-name>
```
to download image from dockerhub

```
docker-compose up
```
to run a container from compose file

```
docker-compose down
```
to delete container

```
docker exec -it <container-id> -- bash 
```
to enter in a container

## volumes 

```
docker volume create <volume-name>
```
to create volume

```
docker volume ls
```
list all the volumes

```
docker volume inspect <name>
```
to inspect any specific volume

```
docker rm <name>
```
to remove volume 

## Network

```
docker network ls
```
to list networks

```
docker network create <name>
```
to create network

```
docker network inspect <name>
```
to remove network

```
docker network connect <net-name> <container-id>
```
to connect network with container

```
docker network disconnect <net-name> <container-id>
```
to disconnect network with container

## clean up 

```
docker system prune
```
Remove unused data (containers, images, volumes, networks)

```
docker image prune
```
remove unused images

```
docker container prune
```
remove unused containers

```
docker network prune
```
remove network containers

```
docker volume prune
```
remove volume containers




