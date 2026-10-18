# Laboratory 06 – Cloud Deployment Engineer

## Mission Overview

This laboratory focuses on deploying a multi-container application using Docker Compose. I created a deployment configuration for Nextcloud and MariaDB. The goal was to understand how application and database containers work together to provide a private cloud storage service.

## Objectives

- Create a project folder and organize the required files.
- Write a `docker-compose.yml` file to define the Nextcloud and MariaDB services.
- Deploy and verify the containers using Docker Compose.
- Access the Nextcloud installation page through port 8080.
- Learn how containers communicate through a Docker network.
- Document the deployment process and understand the difference between Docker commands.

## Commands Executed

| Command | Purpose |
|---|---|
| `mkdir -p Laboratory-06-Cloud-Deployment-Engineer/screenshots` | Creates the project folder and screenshots directory. |
| `mkdir nextcloud-deployment` | Creates the deployment folder. |
| `cd nextcloud-deployment` | Enters the deployment folder. |
| `nano docker-compose.yml` | Creates or edits the Docker Compose configuration. |
| `docker-compose up -d` | Starts the services in the background. |
| `docker-compose ps` | Checks the status of the containers. |
| `docker-compose down` | Stops and removes the Compose containers and network. |
| `ls` | Lists files and folders. |
| `cat docker-compose.yml` | Displays the Compose configuration. |

## Skills Learned

In this laboratory, I learned how to write a Docker Compose configuration and deploy an application with a database. I also learned how the `services` block defines containers and how the `MYSQL_HOST` variable allows Nextcloud to find the MariaDB service through its service name.

I improved my Linux terminal skills by creating folders, editing files, and executing Docker commands. I also learned the importance of checking container status, documenting the deployment, and saving screenshots as evidence of completed tasks.

Overall, this activity helped me understand how multiple containers can work together and how Docker Compose simplifies the deployment of cloud applications.
