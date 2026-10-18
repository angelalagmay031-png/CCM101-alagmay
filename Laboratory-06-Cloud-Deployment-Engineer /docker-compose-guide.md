# Docker Compose Guide

## 1. What Does the `services:` Block Do?

The `services:` block defines the containers that Docker Compose will run. In my YAML file, I created two services: `database` and `app`. The database service uses MariaDB to store the database, while the app service runs Nextcloud. Docker Compose manages these services together, making deployment easier.

## 2. How Does Nextcloud Find the Database?

The Nextcloud container finds the database through the `MYSQL_HOST` environment variable. In my YAML file, I used `MYSQL_HOST=database`. The name `database` matches the database service in the Compose file. Docker Compose creates a network that allows the containers to communicate using their service names. Because of this, Nextcloud can find MariaDB without needing to know its IP address.

## 3. Difference Between `docker run` and `docker-compose up -d`

The `docker run` command starts an individual container. If an application needs multiple containers, I may need to configure and start each container separately.

The `docker-compose up -d` command uses a YAML file to create and start multiple services together. The `-d` option means detached mode, which allows the containers to run in the background while I continue using the terminal.

Docker Compose is more convenient for multi-container applications because the configuration is saved in one file and can be reused.

## Conclusion

Through this activity, I learned how Docker Compose manages multiple containers and connects Nextcloud to MariaDB. I also learned that a YAML configuration makes deployment easier to organize and repeat.
