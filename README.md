# docker-commands

## Docker Containers

### Run Docker Container
```bash
docker run -d -p <host_port>:<container_port> --name <container_name> <image_name>
```

### List all running Docker Containers

```bash
docker ps
```

### List all Docker Containers

```bash
docker ps -a
```

### Stop a specific Docker Container

```bash
docker stop <container_id or container_name>
```

### Remove a stopped Docker Container

```bash
docker rm <container_id or container_name>
```

### Show the logs of a specific Container

```bash
docker logs <container_id or container_name>
```

## Docker Images

### List all downloaded Docker Images

```bash
docker images
```

### Download a specific Docker Image

```bash
docker pull <image_name>
```

### Build Docker Image

```bash
docker build -t <image_name> <path_to_dockerfile>
```

### Upload a specific Docker Image

```bash
docker push <image_name>
```

### Remove a specific Docker Image

```bash
docker rmi <image_id or image_name>
```

## Docker-Compose

### Start a Docker-Compose in detached mode

```bash
docker-compose up -d
```

### Start a specific container of a Docker-Compose in detached mode

```bash
docker-compose up <container_id or container_name> -d
```

### Shut a Docker-Compose dwon

```bash
docker-compose down
```

### Shut a specific container of a Docker-Compose dwon

```bash
docker-compose down <container_id or container_name>
```

### Restart all containers of a Docker-Compose

```bash
docker-compose restart
```

### Restart a specific container of a Docker-Compose

```bash
docker-compose restart <container_id or container_name>
```

### Build all containers of a Docker-Compose

```bash
docker-compose build
```

### Build a specific container of a Docker-Compose

```bash
docker-compose build <container_id or container_name>
```

## Docker System

### Show Docker System information

```bash
docker system info
```

### Remove unused Docker ressources

```bash
docker system prune
```
Removes unused Docker resources, such as stopped containers and dangling images.

### Remove all Docker ressources

```bash
docker system prune -a
```
Removes all Docker resources, including stopped containers, unused networks, and dangling images.

## Docker Network

### List all Docker Networks

```bash
docker network ls
```

### Create a new unique Docker Network

```bash
docker network create <network_name>
```

### Remove a specified Docker Network

```bash
docker network rm <network_id or network_name>
```

## Docker Volumes

### List all Docker Volumes

```bash
docker volume ls
```

### Delete a specific Docker Volume

```bash
docker volume rm <volume_name>
```
