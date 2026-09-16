# Docker Deployment and Container Lifecycle

## Checkpoint 3 - Docker Environment Verification

### 1. Check Docker Version

```bash
docker --version
```

This command displays the installed Docker version and confirms that Docker is available in the environment.

### 2. Check Docker Status

```bash
docker info
```

This command displays detailed information about the Docker environment and confirms that the Docker engine is running.

---

## Checkpoint 4 - Nginx Deployment

### 1. Pull the Nginx Image

```bash
docker pull nginx
```

This command downloads the official Nginx image from Docker Hub to the local Docker environment.

### 2. Run the Nginx Container

```bash
docker run -d --name nginx-server -p 8080:80 nginx
```

This command creates and runs an Nginx container in detached mode and maps host port 8080 to port 80 inside the container.

### 3. Check the Running Container

```bash
docker ps
```

This command lists the containers that are currently running and allows us to verify that the Nginx container is active.

### 4. Test the Web Server

```bash
curl http://localhost:8080
```

This command sends an HTTP request to the Nginx web server through port 8080 and displays the returned HTML content.

The expected response contains the Nginx welcome page.

---

## Checkpoint 5 - Container Lifecycle

### 1. List Running Containers

```bash
docker ps
```

This command displays all currently running Docker containers.

### 2. Stop the Running Container

```bash
docker stop nginx-server
```

This command stops the running Nginx container gracefully.

### 3. Verify the Container Is Stopped

```bash
docker ps -a
```

This command displays all containers, including stopped containers, allowing us to verify that the Nginx container is no longer running.

### 4. Remove the Container Completely

```bash
docker rm nginx-server
```

This command removes the stopped Nginx container from the Docker environment.

### 5. Verify the Container Was Removed

```bash
docker ps -a
```

This command verifies that the Nginx container is no longer listed.

---

## Summary

Docker provides commands that allow users to pull images, create containers, run applications, stop containers, and remove containers. The Nginx deployment demonstrated how a web server can be launched quickly using a container. The container lifecycle commands also demonstrated how a cloud-native engineer manages running and stopped services.

