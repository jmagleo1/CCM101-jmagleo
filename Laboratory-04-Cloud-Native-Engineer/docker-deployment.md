# Docker Deployment

## Docker Commands

| Command | Purpose |
|---|---|
| `docker --version` | Checks the Docker version. |
| `docker info` | Checks the Docker environment. |
| `docker pull nginx` | Downloads the Nginx image. |
| `docker run -d -p 8080:80 --name my-nginx nginx` | Runs the Nginx container and maps the ports. |
| `curl http://localhost:8080` | Tests if Nginx is working. |
| `docker ps` | Shows running containers. |
| `docker stop my-nginx` | Stops the Nginx container. |
| `docker ps -a` | Shows all containers. |
| `docker rm my-nginx` | Removes the stopped container. |

## Summary

I learned how to use basic Docker commands to deploy and manage an Nginx container. I also learned how port mapping works and how to stop and remove a container.
