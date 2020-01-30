#### Check docker version

```bash
docker -v
```


#### Download docker image
```bash
docker pull alpine
```
-> Where alpine is a docker image


#### Run a simple command from the alpine docker image
```bash
docker container run alpine echo "Hello World!"
```

#### Run a command from a container that is not installed
docker container run centos echo "Hello World!"



#### List docker images
```bash
docker images
```

#### View running docker containers
```bash
docker ps
#or
docker container ls
```

#### View all docker containers
```bash
docker ps -a or docker container ls -a
```

#### Start a docker container in the background
```bash
docker container run -d alpine ping host.docker.internal
```


#### Run a container in the background and keep it alive
```bash	
docker container run -di alpine
```

#### Stop a running container
```bash
docker stop container_name_or_id
```

#### Execute a command in a running Docker container where command is `uname -a`
```bash
docker exec -it container_name_or_id uname -a
```


#### Start a shell inside a running container	
```bash
docker exec -it container_name /bin/sh
```

#### Delete a container
```bash
docker rm container_name_or_id
```

#### Force delete a running container 
```bash
docker rm -f container_name_or_id
```

#### Remove a docker image
```bash
docker rmi centos
```

#### Force remove an image
```bash
docker rmi -f centos
```

#### Running a container image with a docker-compose.yml
```bash
docker-compose up -d
```


### Checking the ip address 
```bash
docker inspect container_id or image_id
```



## Networking
```bash
docker network ls
```

### Remove docker network
```bash
docker network rm docker_network_id
```


### Stop and uninstall installed configuration of a docker container (within a directory with docker-compose.yml)
```bash
docker down
```

### Creating a network

`https://docs.docker.com/engine/reference/commandline/network_create/`

```bash
docker network create \
  --driver=bridge \
  --subnet=192.168.0.0/16 \
  --ip-range=192.168.1.0/24 \
  --gateway=192.168.1.254 \
  devnetwork
```

#### SSH into docker container

```bash
docker exec -it 17bbb4179010 bash
```

#### Fix internet access issue from docker container

```bash
vim /etc/resolv.conf 
# connect to 8.8.8.8 
```

#### Connecting foreign container to a docker network

```bash
docker network connect network_name container_name 
```
