# Laboratory 6: The Cloud Deployment Engineer

## Mission Overview

In this mission, I acted as a Cloud Deployment Engineer at CloudNova Technologies. I moved from running single containers with manual commands to Infrastructure as Code, using Docker Compose to deploy a two-tier private cloud storage system (Nextcloud web app and MariaDB database) with a single command.

## Objectives

- Explain the concept of a multi-tier application architecture.
- Understand the purpose and structure of a `docker-compose.yml` file.
- Use the nano text editor to create configuration files.
- Deploy a multi-container application (Nextcloud + MariaDB) using Docker Compose.
- Document deployment procedures and IaC principles using Markdown.
- Continue building my GitHub Cloud Computing Portfolio.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Screenshots

- `screenshots/compose-deployment.png` - Successful deployment and running containers
- `screenshots/nextcloud-web.png` - Nextcloud setup page in the browser
- `screenshots/compose-teardown.png` - Containers stopped and removed

## Skills Learned

- Designing a two-tier architecture
- Writing YAML configuration files
- Deploying and tearing down multi-container stacks with Docker Compose
- Using environment variables and service-name networking
- Exposing an application through a port mapping
- Documenting work in Markdown and using Git/GitHub
