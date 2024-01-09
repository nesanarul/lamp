# LAMP-stack with Docker compose

## Installation
```
git clone git@github.com:nesanarul/lamp.git
cd lamp                               
```

## How to use docker without sudo
Create a docker group and add your user to it. Note that this group will have root-level privileges.
```
sudo groupadd docker
sudo usermod -aG docker $USER
```
## DB
In db the dumb.sql is an sql file containing your sql database export from phpmyadmin. 
Save each time you edit your database before turning off the docker container.
You can do this by going to http://localhost:8001/ logging in with the log in details (visible in docker-compose.yml) and exporting your current database.
### DB User Credentials
Default username: lamp_docker
Default password: password
This can be changed in docker-compose.yml.

## Docker/php
Gets a suitable image + mysql/php connection installations


## How to run
```run in the directory:
docker compose up
```
or for detached mode (no webserver console)
```
docker compose up -d
```
## How to stop
run in the directory:
```
docker compose down
```
## Your site
http://localhost
