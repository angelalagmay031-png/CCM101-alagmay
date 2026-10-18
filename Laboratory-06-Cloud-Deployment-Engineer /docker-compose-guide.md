# Docker Compose Guide

## 1. Introduction

Docker Compose is a tool used to run and manage multiple containers in one application. In this project, I used Docker Compose to deploy Nextcloud and MariaDB. Nextcloud is the application that provides private cloud storage, while MariaDB stores the application's data.

## 2. Explanation of the Services Block

The `services:` block defines the containers that Docker Compose will create and run. In my YAML file, there are two services: `database` and `app`.

- **database:** Uses the `mariadb:10.6` image. It stores the database used by Nextcloud. The environment variables configure the database name, username, and passwords.
- **app:** Uses the `nextcloud` image. It runs the Nextcloud web application and maps port `8080` on the host to port `80` inside the container.

By defining both services in one file, Docker Compose can manage the application and database together.

## 3. How Nextcloud Finds the Database

The Nextcloud container finds the database through the `MYSQL_HOST=database` environment variable. The value `database` matches the name of the database service in the Compose file.

Docker Compose creates a network for the services by default. The containers can communicate through this network using their service names. Therefore, Nextcloud can connect to MariaDB using `database` as the hostname instead of an IP address.

The database connection also uses the same database name, username, and password configured in both services.

## 4. Difference Between docker run and docker-compose up -d

The `docker run` command is commonly used to create and start an individual container with options specified in the command. When running multiple related containers, I may need to configure each container and its network separately.

The `docker-compose up -d` command reads the configuration from `docker-compose.yml` and starts the services defined in the file. It can create the required containers and network and run them in the background because of the `-d` option.

In this project, Docker Compose is more convenient because it manages the Nextcloud application and MariaDB database together using one configuration file.

## 5. Conclusion

Through this activity, I learned how Docker Compose organizes multiple services, how containers communicate using service names, and how environment variables configure an application. I also learned that Docker Compose makes multi-container deployment easier to manage and repeat.
