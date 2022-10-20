---
sidebar_position: 1
---
----
# Useful Docker Commands
----

### 1. Docker install & update 

```bash
sudo apt update -y ; sudo apt upgrade -y; sudo apt autoremove -y; sudo apt install docker-compose -y
```

### 2. Docker up and build

```bash
sudo docker-compose up --build
```

### 3. Cleaning all docker files

```bash
docker system prune -f -a
```

### 4. Docker Stop command 

```bash 
docker stop container name/image id 
```


### 5. Docker Storage 

```bash 
docker system df
docker system df -v

```


### 6. Docker Remove & stop all container 

```bash 
docker rm -f $(docker ps -a -q)

```

### 7. Docker image build 

```bash
DOCKER_BUILDKIT=1 docker build -t "dockerusername/imagename:version" .

DOCKER_BUILDKIT=1 docker build -t "dockerusername/imagename:version" github.com/username/repo

DOCKER_BUILDKIT=1 docker build -t "dockerusername/imagename:version" -t "dockerusername/imagename:latest" . #for multiple tags with versioning and latest 

```

### 8. How to push Docker Image to DockerHub

```bash
docker login #user your creds to login 
docker push dockerusername/imagename:version #same as you have used in Buildkit
docker push dockerusername/imagename --all-tags #For all versions 
```

### 9. How to view Docker image content

```bash
docker image history --no-trunc image name/image id 
```
