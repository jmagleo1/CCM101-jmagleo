# Mission Reflection

Writing a `docker-compose.yml` file makes a cloud engineer's job easier because it allows multiple containers to be configured and deployed using one file. Instead of manually typing many Docker commands and configuring each container one by one, Docker Compose can create and connect the services automatically. This makes the deployment faster, more organized, and easier to repeat.

If there is an indentation error in a YAML file, the configuration may not work correctly. YAML depends on proper spaces and indentation to understand the structure of the file. For example, using a Tab instead of spaces can cause an error when Docker Compose reads the file. This taught me that even small formatting mistakes can affect the whole deployment.

We used environment variables such as `MYSQL_PASSWORD` to provide the database settings needed by Nextcloud. They allow the containers to receive important configuration values without putting those settings directly into the application commands. It also makes the configuration easier to manage when settings need to be changed.

Deploying Nextcloud in just a few minutes felt exciting because I was able to see how cloud technologies can make deployment much faster. Before this activity, I thought setting up a cloud storage system would require many complicated steps. Using Docker Compose made it possible to deploy the application and database together with only a few commands.

Since Mission 1, my understanding of Cloud Computing has improved a lot. I learned that cloud computing is not only about using online storage or applications. It also involves virtualization, containers, cloud services, networking, storage, and deployment. Through these missions, I became more familiar with using Linux, Docker, and cloud-related tools. I also learned that automation and proper configuration are important skills for a cloud engineer.
