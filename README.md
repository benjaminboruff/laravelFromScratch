## Follow along with Jeff Way's `Laravel 5.7 From Scratch` Laracast series 

#### No need to install `composer` since it is already in the docker image.

1. Step One: git clone the repo and checkout step_1, then bash into the web service

    > docker-compose run --rm -u $(id -u):$(id -g) web bash

    In the `web` container run:

    > composer global require "laravel/installer"

    > laravel new myfirstsite

    After it has completed, exit the container.

2. Step Two: checkout step_2 and run the app

    > env UID=$(id -u) GID=$(id -g) docker-compose up
