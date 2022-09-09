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
