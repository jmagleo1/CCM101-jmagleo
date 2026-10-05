# Docker Compose Guide

## What Does the `services:` Block Do?

The `services:` block is used to define the containers needed for the application. In our Docker Compose file, we have two services: `database` and `app`.

The `database` service uses the MariaDB 10.6 image, which is responsible for storing the data needed by Nextcloud. The `app` service uses the Nextcloud image and provides the web application that users can access through the browser.

## How Did the Nextcloud App Container Find the Database?

The Nextcloud app container was able to find the database container because of the `MYSQL_HOST` environment variable.

In our Compose file, it is set as:

    MYSQL_HOST=database

The word `database` is the name of the MariaDB service. Docker Compose allows containers in the same network to communicate using their service names. Because of this, Nextcloud was able to find and connect to the MariaDB container using `database` as the host.

## Difference Between `docker run` and `docker-compose up -d`

The `docker run` command is mainly used to create and start one Docker container. In Mission 4, we used Docker commands to work with individual containers, so each container had to be managed separately.

The `docker-compose up -d` command works differently because it uses the `docker-compose.yml` file to create and start multiple services at the same time. In this mission, one command started both the Nextcloud application and MariaDB database containers.

The `-d` option means that the containers run in the background. This allows us to continue using the terminal while the containers are running.

## Summary

Docker Compose made the deployment easier because the configuration for the Nextcloud application and MariaDB database was written in one YAML file. Instead of manually creating and connecting each container, Docker Compose handled the services and their network connection based on the configuration.
