#### Check docker version
docker -v


#### Download docker image
docker pull alpine

-> Where alpine is a docker image


#### Run a simple command from the alpine docker image
docker container run alpine echo "Hello World!"

#### Run a command from a container that is not installed
docker container run centos echo "Hello World!"



#### List docker images
docker images

#### View running docker containers
docker ps or docker container ls


#### View all docker containers
docker ps -a or docker container ls -a

#### Start a docker container in the background
docker container run -d alpine ping host.docker.internal


#### Run a container in the background and keep it alive	
docker container run -di alpine

#### Stop a running container
docker stop container_name_or_id


#### Execute a command in a running Docker container where command is `uname -a`
docker exec -it container_name_or_id uname -a



#### Start a shell inside a running container	
docker exec -it container_name /bin/sh

#### Delete a container
docker rm container_name_or_id

#### Force delete a running container 
docker rm -f container_name_or_id

#### Remove a docker image
docker rmi centos

#### Force remove an image
docker rmi -f centos