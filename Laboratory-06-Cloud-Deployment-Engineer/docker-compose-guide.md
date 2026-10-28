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

The named volumes `db_data` and `nextcloud_data` store database and Nextcloud files beyond the lifecycle of an individual container.

## Docker Commands

| Command | Purpose |
|---|---|
| `docker-compose config` | Checks and displays the Compose configuration |
| `docker-compose up -d` | Starts the services in the background |
| `docker-compose ps` | Shows the service container status |
| `docker-compose down` | Stops and removes the containers and Compose network |

## Docker Run vs. Docker Compose

The `docker run` command starts an individual container with options supplied on the command line. The `docker-compose up -d` command reads a Compose YAML file and starts the services defined in it, making a multi-container setup easier to manage.
