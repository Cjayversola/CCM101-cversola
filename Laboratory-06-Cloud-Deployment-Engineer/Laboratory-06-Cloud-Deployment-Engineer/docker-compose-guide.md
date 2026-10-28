# Docker Compose Guide

## What Is Docker Compose?

Docker Compose is a tool that defines and runs multiple containers using a YAML configuration file. In this activity, I used it to manage Nextcloud and MariaDB together.

## Important Configuration Parts

### `services:`

The `services:` section defines the containers that make up the application. I created two services: `app` for Nextcloud and `database` for MariaDB.

### `MYSQL_HOST=database`

This environment variable tells Nextcloud the hostname of its database service. Docker Compose allows the application container to reach the database through the service name `database`.

### Port Mapping

The configuration uses `8080:80`. This maps port 8080 on the host to port 80 inside the Nextcloud container, allowing me to open the web application through port 8080.

### Volumes

The named volumes `db_data` and `next
