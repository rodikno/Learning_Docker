# Learning_Docker

`docker ps` - view all running containers
`docker ps -a' - view containers run history

`docker build -t learn-docker-php .` - build an image from Dockerfile located in the current directoty (image will have name `learn-docker-php`)
`docker run -p 80:80 -v C:\_projects\Learning_Docker\src\:/var/www/html learn-docker-php` - create a container from image `learn-docker-php`, container will have port 80 open and binded with port 80 on localhost (host machine), also mount folder `C:\_projects\Learning_Docker\src\` to `/var/www/html` so container will look at it in the realtine and all changes will be reflected
`docker stop [CONTAINER_ID]` - kills container with id `CONTAINER_ID`, which could be retrieved from `docker ps` command
