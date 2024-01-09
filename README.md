# LAMP-stack with Docker compose

# DB
In db the dumb.sql is an sql file containing your sql database export from phpmyadmin. 
Save each time you edit your database before turning off the docker container.
You can do this by going to http://localhost:8001/ logging in with the log in details (visible in docker-compose.yml) and exporting your current database.

# Docker/php
Gets a suitable image + mysql/php connection installations


# How to run
run in the directory:
docker compose up

# How to stop
run in the directory:
CTRL + C
docker compose down
