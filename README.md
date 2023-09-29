
# Ready To Use Full Stack Docker Environment
## Installation Instructions:
Clone this repository to your desired location:
```
git clone https://github.com/cljamal/DockerFullStackWebServer.git
```

Next, navigate to the project directory and run the following command to build and start the Docker containers:
```
cd DockerFullStackWebServer
docker-compose build && docker-compose up -d
```
After completing these steps, you will have the following services accessible:

PHP Project: http://localhost:8080
Adminer (MySQL Database Management): http://localhost:8090
Portainer (Container Management): http://localhost:9000
Node.js Project 1: http://localhost:3000
Node.js Project 2: http://localhost:3000
Redis Port: localhost:9091

You can configure the settings for all these services in either the ```docker-compose.yml``` file or the ```.env```(don't forget create ```.env``` from ```.env.example```) file.

> Note: Nginx is running using the trafex/php-nginx Docker image. For
> the PHP server, you can customize the configurations for Nginx and
> PHP, which are located in ```./Containers/PHP/nginx``` and
> ```./Containers/PHP/php```. Feel free to adjust them according to your
> preferences.