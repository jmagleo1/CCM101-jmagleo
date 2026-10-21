# Laboratory 10 - Enterprise Cloud Architect

## Mission Overview

In this laboratory activity, I worked as an Enterprise Cloud Architect for CloudNova Technologies. I created a cloud setup using Ubuntu Server in VirtualBox and deployed Ghost and MySQL using Docker and Docker Compose. I also configured persistent storage to keep the data safe, set up the UFW firewall to protect the server, and created a Bash script to automate database backups using cron jobs.

This activity helped me apply the knowledge and skills I learned from our previous Cloud Computing laboratory activities.

## Objectives

- Create an architecture diagram for the cloud infrastructure.
- Set up an Ubuntu Server virtual machine using VirtualBox.
- Install and use Docker and Docker Compose.
- Deploy Ghost and MySQL containers.
- Use persistent volumes to keep application and database data.
- Configure UFW to control incoming network connections.
- Create a Bash script for database backups.
- Schedule automatic backups using cron.
- Test the backup and recovery process.
- Organize and document the project in my GitHub portfolio.

## Technologies Used

- Ubuntu Server
- Oracle VirtualBox
- Docker and Docker Compose
- Ghost
- MySQL
- UFW Firewall
- Bash Scripting
- Cron
- SSH
- Markdown and GitHub

## Commands Executed

| Command | Purpose |
|---|---|
| `ssh -p 2222 vin@127.0.0.1` | Connect to the Ubuntu Server VM. |
| `docker compose pull` | Download the required Docker images. |
| `docker compose up -d` | Start the application containers in the background. |
| `docker compose ps` | Check the status of the containers. |
| `docker compose down` | Stop and remove the containers without deleting persistent volumes. |
| `sudo ufw status verbose` | Check the firewall status and rules. |
| `sudo ss -tulpn` | Check the ports being used by running services. |
| `./automation-script.sh` | Run the database backup script. |
| `ls -lh ~/backups` | Check the backup files and their sizes. |
| `cat ~/backups/backup.log` | View the backup activity log. |
| `crontab -l` | Check the scheduled cron jobs. |
| `docker volume ls` | View the available Docker volumes. |
| `sudo reboot` | Restart the Ubuntu Server VM. |

## Skills Learned

- Creating a simple cloud infrastructure design.
- Deploying applications using Docker and Docker Compose.
- Using Docker volumes to preserve important data.
- Securing a Linux server with the UFW firewall.
- Checking open ports and running services.
- Writing a Bash script for database backups.
- Scheduling automatic tasks using cron.
- Learning how database backups can be restored.
- Checking if containers work properly after a server restart.
- Writing technical documentation using Markdown.

## Files

- [Architecture Diagram](https://github.com/just-berry-th1ngs/CCM101-jlagmay/blob/main/Laboratory-10-Enterprise-Cloud-Architechture/architecture-diagram.png)
- [Docker Compose Configuration](https://github.com/just-berry-th1ngs/CCM101-jlagmay/blob/main/Laboratory-10-Enterprise-Cloud-Architechture/docker-compose.yml)
- [Automation Script](https://github.com/just-berry-th1ngs/CCM101-jlagmay/blob/main/Laboratory-10-Enterprise-Cloud-Architechture/automation-script.sh)
- [Operational Manual](https://github.com/just-berry-th1ngs/CCM101-jlagmay/blob/main/Laboratory-10-Enterprise-Cloud-Architechture/operational-manual.md)
- [Final Reflection](https://github.com/just-berry-th1ngs/CCM101-jlagmay/blob/main/Laboratory-10-Enterprise-Cloud-Architechture/final-reflection.md)

## Project Summary

This laboratory activity helped me understand how the different topics in Cloud Computing work together. I was able to apply what I learned about Linux, virtual machines, Docker, networking, security, and automation. I also learned the importance of keeping data safe through persistent storage and regular backups.

Overall, this activity gave me more experience in setting up and managing a cloud application. It also helped me understand the responsibilities of a cloud architect, especially in maintaining security, keeping services available, and preparing for possible system problems.
