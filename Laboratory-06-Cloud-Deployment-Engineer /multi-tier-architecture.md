# Two-Tier Architecture

## What Is a Two-Tier Architecture?

A two-tier architecture is a system design that separates an application into two main parts: the web/application tier and the database tier. Each tier has a different responsibility, but they communicate with each other to provide the required service. In this laboratory, Nextcloud serves as the application, while MariaDB stores the database information.

## The Web/Application Tier

The web/application tier handles user requests and provides the interface that users access through a web browser. In this project, the Nextcloud container runs the application and makes its web interface available through port 8080. It communicates with the database to retrieve and store information.

## The Database Tier

The database tier stores persistent information needed by the application, such as database records and account-related information. In this project, MariaDB runs in a separate container and uses the database name `nextcloud_db` and the user `nextcloud_user`. The Nextcloud application connects to MariaDB to access the information it needs.

## Why Separate Them?

Separating the web server and database into two containers makes the system easier to manage, update, and troubleshoot. It also allows each service to be configured and scaled independently. If the application needs an update, the database can remain a separate service instead of having both components packed into one container.

## Conclusion

The two-tier architecture used in this laboratory demonstrates how different services can work together in a cloud environment. Nextcloud handles the application, while MariaDB manages the database. Docker Compose helps define and manage both services through a single configuration file.
