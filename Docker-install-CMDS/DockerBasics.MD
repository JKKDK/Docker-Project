### Docker Commands
* To pull the image from Docker Hub. If you dont mention version it will pull the latest version by default.
```
docker pull [image-name]:[version]
```
* To display the available images
```
docker images
```
* To create container out of image
```
docker create [image-id]
```
* To display the running containers.
```
docker ps
```
* To display all running and stopped containers.
```
docker ps -a
```
* To start the container
```
docker start [container-ID]
```
* To pull, create and start the container with single command
```
docker run [image-name]:[version]
```
* By default docker containers run in the foreground attached to the screen. If you want to detach use -d
```
docker run -d [image-name]:[version]
```
* To assign a port to the container
```
docker run -d -p [host-port]:[container-port] [image-name]:[version]
```
* To name the container
```
docker run -d --name [name-you-wish] [image-name]:[version]
```
* To login the container shell. To come out use CTRL+d
```
docker exc -it [container-id] bash
```
* To stop the running container
```
docker stop [container-ID]
```
* To remove the container. If it is running container use -f to force
```
docker rm [container-ID]
```
* To remove images
```
docker rmi [image-ID]
```
*  To display command executed at the time of container creation
```
docker ps --no-trunc 
```
* Only to display all the stopped and running container IDs
```
docker ps -a -q
```
* To Remove all the containers at a time
```
docker rm -f `docker ps -a -q` 
```








