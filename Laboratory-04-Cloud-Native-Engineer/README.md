# Laboratory 04 - Cloud-Native Engineer

## Mission Overview

This laboratory activity introduced the concept of containerization and demonstrated how Docker can be used to deploy and manage a containerized web server. Using the KillerCoda Docker Playground, I verified Docker, pulled the official Nginx image, ran an Nginx container, tested the web server, and managed the container lifecycle.

## Objectives

The objectives of this laboratory activity were to:

- Differentiate between traditional Virtual Machines and Containers.
- Access a Docker-enabled cloud environment using KillerCoda.
- Execute fundamental Docker CLI commands.
- Pull, run, manage, and terminate a containerized Nginx application.
- Document container operations using Markdown.
- Continue developing a well-organized GitHub Cloud Computing portfolio.

## Docker Commands Executed

### Docker Environment Verification

docker --version
docker info

### Nginx Deployment

docker pull nginx
docker run -d --name nginx-server -p 8080:80 nginx
docker ps
curl http://localhost:8080

### Container Lifecycle

docker ps
docker stop nginx-server
docker ps -a
docker rm nginx-server
docker ps -a

### Skills Learned

Through this activity, I learned how to use Docker commands in a Linux environment. I learned how to verify Docker, pull a Docker image, create and run a container, map a host port to a container port, test a web server, stop a container, and remove a container. I also learned how to document technical procedures using Markdown and organize screenshots as evidence in a GitHub repository.

### Challenges Encountered

One challenge I encountered was becoming familiar with the Docker command-line interface and understanding the purpose of each command. Another challenge was verifying that the Nginx web server was accessible through port 8080. Checking the Docker container status and testing the server using curl helped me understand how container deployment works.

### Screenshots

The screenshots for this laboratory activity are stored in the screenshots folder.

docker-version.png - Docker installation and environment verification
nginx-running.png - Successful Nginx web server response
container-lifecycle.png - Docker container lifecycle commands
