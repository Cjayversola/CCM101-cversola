# Multi-Tier Architecture

## Overview

In this activity, I deployed Nextcloud and MariaDB using Docker Compose. The setup has two main tiers: the web application tier and the database tier.

## Web/Application Tier

The application tier uses the Nextcloud Docker image. It provides the web interface that users access through a browser. Port 8080 on the host is mapped to port 80 inside the container.

## Database Tier

The database tier uses MariaDB 10.6 to store application data. The database service is named `database`, and Nextcloud connects to it using `MYSQL_HOST=database`.

## Why Separate the Tiers?

Separating the application and database makes the services easier to manage and update independently. It also allows each service to have its own configuration and persistent storage.

## Services Used

- **Nextcloud:** Web application and user interface.
- **MariaDB:** Database service.
- **Docker Compose:** Defines and manages both services.
