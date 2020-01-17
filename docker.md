### Standard commands
run a container
```
docker run -d --hostname my-rabbit --name local-rabbit -p 8080:15672 rabbitmq:3-management
```
inspect a container
```
docker inspect local-rabbit
```
show all active containers
```
docker ps
```
show all containers even stopped one
```
docker ps --all
```
start an existing container
```
docker start local-rabbit
```
stop an existing container
```
docker stop local-rabbit
```
remove a container
```
docker rm local-rabbit (or using container-id)
```
show docker images
```
docker images
```
remove a docker image
```
docker rmi <NAME or ID>
```

### Enter in a container
```
docker exec -it local-rabbit bash
```

### Create an image and publish it to dockerhub
create *Dockerfile* with what you want

in the same folder of docker file (or in a folder that you have to explicit)
```
docker build -t <image-name> .
```
tag a container with your dockerhub username
```
docker tag <image-name> <dockerhub_user>/<image-name>
```
login to dockerhub
```
docker login
```
push image to dockerhub
```
docker push <dockerhub_user>/<image-name>
```
