# Mission Reflection

In this laboratory activity, I learned that Docker containers can be started much faster than a Virtual Machine. A VM usually needs a complete operating system to be installed and started, which uses more time and resources. A Docker container already uses an existing image, so it can start in only a few seconds. This makes containers useful when applications need to be deployed quickly.

The port mapping -p 8080:80 is necessary because the Nginx web server is running inside the container on port 80. Port 8080 allows the host system to access the web server from outside the container. When I used curl http://localhost:8080, the request was forwarded to port 80 of the Nginx container. The successful Welcome to nginx! output showed that the port mapping was working correctly.

When docker rm is used, the container itself is permanently removed. Any data stored only inside the container can be lost after it is removed. This is why important data should be stored using Docker volumes or another persistent storage method instead of keeping it only inside the container.

Containerization can also change how developers and IT operations teams work together. Developers can create applications in consistent environments, while operations teams can deploy and manage those applications more easily. This supports the DevOps approach because both teams can work with the same containerized application setup.

My GitHub portfolio is also improving as I add more laboratory activities. In this activity, I added my Docker commands, comparison of VMs and containers, and reflection. It helps me keep my cloud computing activities organized and shows the skills I have learned throughout the course.
