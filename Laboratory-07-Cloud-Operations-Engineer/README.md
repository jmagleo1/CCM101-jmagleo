# Mission 7: The Cloud Operations Engineer

## Mission Overview

In this laboratory activity, I worked as a Cloud Operations Engineer for CloudNova Technologies. I checked the Linux server resources, deployed an Nginx container, generated web traffic, checked application logs, and monitored the container's CPU and memory usage.

## Objectives

- Monitor the CPU, memory, and disk resources of a Linux server.
- Deploy an Nginx web server using Docker.
- Generate successful and failed HTTP requests.
- Analyze Docker application logs.
- Monitor real-time container CPU and memory usage.
- Document the server health and container performance.

## Monitoring Commands Executed

The following Linux and Docker commands were used during the activity:

    free -h
    df -h /
    top
    docker run -d --name client-website -p 8080:80 nginx
    docker ps
    curl http://localhost:8080
    curl http://localhost:8080/hidden-admin-page
    docker logs client-website
    docker stats

## Skills Learned

This activity helped me improve my skills in Linux system monitoring, Docker container management, web server deployment, log analysis, and performance monitoring. I also learned how to use actual system data and container metrics to check if a web application is running properly.
