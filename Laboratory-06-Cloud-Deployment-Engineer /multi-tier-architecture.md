# Two-Tier Architecture

## What Is a Two-Tier Architecture?

A two-tier architecture is a system design that separates an application into two main parts: the web/application tier and the database tier. These two tiers communicate with each other to provide services to users. In this project, Nextcloud is the application, while MariaDB is the database.

## The Web/Application Tier

The web/application tier provides the user interface and handles HTTP requests from users. In this laboratory, the Nextcloud container runs the cloud storage application and allows users to access its web interface through port 8080. It communicates with the database to retrieve and store information.

## The Database Tier

The database tier stores persistent data used by the application, including database records and account-related information. In this project, MariaDB runs in a separate container and uses the database name `nextcloud_db` and the username `nextcloud_user`.

## Why Separate Them?

Separating the web server and database into two containers makes the system easier to manage, update, and troubleshoot. Each container has its own responsibility, so the application can be updated without placing the database in the same container. This design also makes it easier to maintain and scale each service independently.
