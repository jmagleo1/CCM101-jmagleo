# Laboratory 04 – The Cloud-Native Engineer

## Mission Overview

For this laboratory, I explored how containerization is used in a cloud-native environment. I first compared Virtual Machines and containers to understand their differences in terms of setup, performance, resources, and isolation. After that, I used KillerCoda and Docker to deploy an Nginx web server, test it locally, and manage its container lifecycle.

## Objectives

- Understand the basic differences between VMs and containers.
- Use a Docker-enabled environment through KillerCoda.
- Practice common Docker CLI commands.
- Deploy an Nginx web server using a container.
- Learn how port mapping works in Docker.
- Manage and remove a Docker container.
- Document the activity in my GitHub portfolio.

## Docker Commands Executed

### Docker Setup

- `docker --version`
- `docker info`

### Nginx Deployment

- `docker pull nginx`
- `docker run -d -p 8080:80 --name my-nginx nginx`
- `curl http://localhost:8080`

### Container Management

- `docker ps`
- `docker stop my-nginx`
- `docker ps`
- `docker rm my-nginx`
- `docker ps -a`

## Skills Learned

This activity gave me hands-on experience with Docker instead of only learning about containers through theory. I learned how to get an image from Docker Hub, create and run a container, connect its port to the host machine, and manage the container from start to finish. I also became more familiar with using the terminal and writing technical documentation in Markdown.

## Challenges Encountered

One of the things I had to understand carefully was how Docker port mapping works, especially the `8080:80` format. I also needed to make sure that I was using the correct container name when stopping and removing it. After following the commands and checking the results in the terminal, I was able to complete the deployment and container management tasks.
