# Mission Reflection

This laboratory helped me understand the difference between Virtual Machines and Docker containers. When using a Virtual Machine, a complete operating system needs to be installed and started before an application can be used. This usually takes more time and uses more RAM and storage. In comparison, a Docker container can start within seconds because it shares the host operating system and only contains the application and its needed dependencies.

The port mapping `-p 8080:80` is necessary because the Nginx web server is running inside the container. Port 80 is the port used by Nginx inside the container, while port 8080 is the port exposed on the host machine. Because of this mapping, I was able to access the Nginx web server using `curl http://localhost:8080`.

I also learned that using `docker rm` removes the container from Docker. Data that is stored only inside the container can be lost when the container is removed, so important data should be stored using persistent storage when needed.

Containerization can improve the way software developers and IT operations teams work together. Developers can package applications together with their dependencies, while the operations team can deploy the same container in different environments. This can make deployment more consistent and support the DevOps workflow.

My GitHub portfolio is also improving as I complete each laboratory activity. I started with basic cloud concepts and research, and now I am adding practical Docker commands, deployment activities, screenshots, and technical documentation. This laboratory gave me more hands-on experience and helped me understand how cloud-native technologies are used.
