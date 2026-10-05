# Mission Reflection

## Reflection

Checking the host resources is important even if the containers are working properly because the containers still use the server's CPU, RAM, and disk space. If the server does not have enough resources, the containers may become slow or stop working properly. That is why it is important to check the server first.

The `docker logs` command is helpful when trying to find problems in an application. It shows the requests and errors that happen inside the container. In this activity, I was able to see the 404 error from the request to the hidden page. This helped me understand what happened instead of just guessing the problem.

Logs and metrics are different from each other. Logs show the events, requests, and errors that happened in the application. Metrics show numbers about the performance of the container, such as CPU and memory usage. For example, I used `docker stats` to check the CPU and memory used by the Nginx container.

For companies that have thousands of containers, checking them one by one would be difficult. They can use monitoring tools like Prometheus to collect information and Grafana to display the information in dashboards. These tools can help engineers monitor many containers and find problems faster.

This activity improved my Linux troubleshooting skills because I learned how to check server resources using `free`, `df`, and `top`. I also learned how to use Docker commands to run a container, check logs, and monitor its resources. I became more comfortable using the terminal and understanding the information shown by the commands. Overall, this activity helped me understand how Cloud Operations Engineers monitor and troubleshoot servers and containers.
