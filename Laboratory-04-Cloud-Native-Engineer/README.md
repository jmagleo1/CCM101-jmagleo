# Laboratory 04 – The Cloud-Native Engineer

## Mission Overview

In this laboratory, I learned the difference between Virtual Machines and containers. I also used KillerCoda to practice Docker commands and deploy an Nginx web server using a container.

## Objectives

- Differentiate Virtual Machines and Containers.
- Use a Docker-enabled cloud environment.
- Execute basic Docker commands.
- Pull, run, manage, and remove an Nginx container.
- Document Docker operations using Markdown.
- Continue developing my GitHub Cloud Computing Portfolio.

## Docker Commands Executed

### Checkpoint 3 – Docker Verification

```bash
docker --version
docker info
Checkpoint 4 – Nginx Deployment
docker pull nginx
docker run -d -p 8080:80 --name my-nginx nginx
curl http://localhost:8080
Checkpoint 5 – Container Lifecycle
docker ps
docker stop my-nginx
docker ps
docker rm my-nginx

## Skills Learned

I learned how to use basic Docker commands, deploy an Nginx container, map ports, and manage the container lifecycle. I also improved my skills in writing technical documentation using Markdown.

## Challenges Encountered

My main challenge was understanding the Docker commands and the port mapping -p 8080:80. By following the commands step by step and checking the terminal output, I was able to complete the activity.
