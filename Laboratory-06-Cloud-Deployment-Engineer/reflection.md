# Reflection

In this activity, I learned how Docker Compose can make deploying an application easier. Instead of starting Nextcloud and MariaDB separately with long commands, I used one YAML file to define both services. The `docker-compose up -d` command started the containers in the background, while `docker-compose ps` helped me check their status.

One challenge was making sure the YAML file had the correct indentation and structure. YAML depends on spacing, so an indentation mistake can cause a configuration error. I used `docker-compose config` to check the configuration before deploying it.

I also learned the purpose of environment variables. For example, `MYSQL_HOST=database` tells Nextcloud which database service to connect to. The database username, password, and database name must also match the settings configured for MariaDB.

It was satisfying to see Nextcloud running in the browser after setting up the containers. I was able to access the dashboard through port 8080 and then stop the deployment using `docker-compose down`. This activity helped me understand how different services can work together in a single application.

Compared with the earlier cloud activities, I now have a better understanding of how containers can be used to deploy applications. I also learned that configuration files make deployments easier to repeat and manage.
