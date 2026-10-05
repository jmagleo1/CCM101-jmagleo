# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

In this laboratory, I deployed a private cloud storage system using Nextcloud and Docker Compose. The project used a two-tier architecture with a Nextcloud application container and a MariaDB database container.

I created a `docker-compose.yml` file to configure the two containers and used Docker Compose to deploy them together. I also accessed the Nextcloud setup page through port 8080 to check if the deployment was working properly.

## Objectives

- Understand the basic concept of two-tier architecture.
- Create a Docker Compose configuration file.
- Deploy Nextcloud and MariaDB using Docker Compose.
- Connect the Nextcloud application to the MariaDB database.
- Access the Nextcloud web interface through port 8080.
- Learn how Docker Compose simplifies multi-container deployment.
- Practice using Infrastructure as Code through a YAML file.

## Commands Executed

    mkdir nextcloud-deployment
    cd nextcloud-deployment
    nano docker-compose.yml
    cat docker-compose.yml
    docker-compose up -d
    docker-compose ps
    docker-compose down

## Skills Learned

In this laboratory, I learned how to use Docker Compose to deploy multiple containers as one application. I learned how the Nextcloud container communicates with the MariaDB container using the service name `database`.

I also learned how to create a YAML configuration file and use environment variables for container settings. This activity helped me understand how Infrastructure as Code can make cloud deployment easier, organized, and repeatable.
