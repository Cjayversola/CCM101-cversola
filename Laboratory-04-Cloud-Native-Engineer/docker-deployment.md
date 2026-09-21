# Docker Deployment

## Docker Commands

### 1. Pull the Nginx Image

docker pull nginx

This downloads the official Nginx image that will be used to create the container.

### 2. Run the Nginx Container

docker run -d --name nginx-server -p 8080:80 nginx

This runs the Nginx container in detached mode and maps port 8080 on the host to port 80 inside the container.

### 3. Test the Web Server

curl http://localhost:8080

This sends a request to the Nginx web server and confirms that it is working.

### 4. List Running Containers

docker ps

This displays the containers that are currently running.

### 5. Stop the Container

docker stop nginx-server

This stops the running Nginx container.

### 6. Verify the Container Status

docker ps

This checks the running containers and confirms that nginx-server is no longer running.

### 7. View All Containers

docker ps -a

This displays both running and stopped containers.

### 8. Remove the Container

docker rm nginx-server

This removes the Nginx container from the Docker environment.

### 9. Final Verification

docker ps -a

This confirms that the nginx-server container has been removed.
