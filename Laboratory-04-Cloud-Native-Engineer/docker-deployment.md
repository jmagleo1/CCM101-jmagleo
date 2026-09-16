# Docker Deployment

## Container Lifecycle

### 1. List Running Containers

```bash
docker ps
This command lists all Docker containers that are currently running.

2. Stop the Running Container
docker stop my-nginx

This command stops the running Nginx container named my-nginx.

3. Verify It Is Stopped
docker ps

This command verifies that the my-nginx container is no longer running.

4. Remove the Container Completely
docker rm my-nginx

This command completely removes the stopped my-nginx container from Docker.
