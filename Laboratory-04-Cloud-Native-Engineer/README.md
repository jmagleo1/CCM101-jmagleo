# Laboratory 04 – The Cloud-Native Engineer

## Mission Overview

In this laboratory activity, I took on the role of a Cloud-Native Engineer at CloudNova Technologies. The main task was to understand the difference between traditional Virtual Machines and containers. I also used the KillerCoda Playground to practice Docker commands and deploy an Nginx web server inside a container. Through this activity, I was able to experience how containerization can make application deployment faster and more lightweight.

## Objectives

- Differentiate between traditional Virtual Machines (VMs) and Containers.
- Access a Docker-enabled environment using KillerCoda.
- Execute basic Docker CLI commands.
- Pull and run an Nginx container.
- Use port mapping to access a web server.
- Manage and remove a running container.
- Create technical documentation using Markdown.
- Continue developing my GitHub Cloud Computing Portfolio.

## Docker Commands Executed

### Docker Verification

- `docker --version`
- `docker info`

### Nginx Deployment

- `docker pull nginx`
- `docker run -d -p 8080:80 --name my-nginx nginx`
- `curl http://localhost:8080`

### Container Lifecycle

- `docker ps`
- `docker stop my-nginx`
- `docker ps`
- `docker rm my-nginx`
- `docker ps -a`

## Skills Learned

Through this laboratory activity, I learned how to use Docker and manage a basic containerized application. I learned how to pull an image from Docker Hub, run an Nginx container in detached mode, and use port mapping to access the web server. I also practiced checking running containers, stopping a container, and removing it using Docker CLI commands.

## Challenges Encountered

One challenge I encountered was becoming familiar with the Docker commands because this was my first time performing these container operations. I also needed to understand the port mapping syntax `-p 8080:80` and which port belongs to the host and the container. By following the commands step by step and checking the terminal output, I was able to understand the process better and complete the activity.
