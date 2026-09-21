# Mission 4: The Cloud-Native Engineer

## Mission Overview

In this laboratory activity, I learned how containers are used in cloud computing. I compared Virtual Machines and containers and used Docker in the KillerCoda environment to deploy an Nginx web server.

## Objectives

- Differentiate Virtual Machines and containers.
- Verify that Docker is installed and running.
- Pull and run an Nginx container.
- Map a host port to a container port.
- Manage the lifecycle of a Docker container.
- Document Docker operations using Markdown.

## Docker Commands Executed

docker --version
docker info
systemctl status docker --no-pager
docker pull nginx
docker run -d --name nginx-server -p 8080:80 nginx
curl http://localhost:8080
docker ps
docker stop nginx-server
docker ps
docker ps -a
docker rm nginx-server
docker ps -a

## Skills Learned

I learned how to use basic Docker commands to run and manage containers. I also learned how to deploy and test an Nginx web server.

## Challenges Encountered

My main challenge was understanding the Docker commands and port mapping. I was able to solve it by following the commands and checking the output after each step.
