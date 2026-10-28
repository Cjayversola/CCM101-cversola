# Laboratory 06 - Cloud Deployment Engineer

## Mission Overview

In this activity, I deployed Nextcloud and MariaDB using Docker Compose in the KillerCoda Ubuntu Playground. I also checked the containers, opened Nextcloud in a browser, and stopped the deployment after testing.

## Objectives

- Understand a basic multi-tier application architecture.
- Create a Docker Compose configuration.
- Deploy Nextcloud and MariaDB containers.
- Access the Nextcloud web interface.
- Stop the deployment and document the process.

## Commands Executed

```bash
mkdir -p ~/nextcloud-deployment
cd ~/nextcloud-deployment
docker --version
docker-compose --version
docker-compose config
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

I learned how to define services in a Docker Compose YAML file, connect an application to a database, map a container port to a host port, and check the status of containers. I also learned how Docker Compose makes deploying and stopping a multi-container application easier.
