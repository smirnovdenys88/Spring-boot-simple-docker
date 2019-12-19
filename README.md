1)check docker ( docker --version  ) if not docker install docker for ubuntu (sudo apt-get update)
2) check docker (docker-composer --version) if not install docker-composer ()

docker build -t springio/gs-spring-boot-docker .
$ docker build --build-args DEPENDENCY=build/dependency -t springio/gs-spring-boot-docker .
docker run -p 8080:8080 -t spring-boot-docker

In this project, the following start docker procedure
1) docker compose start try command -> docker-compose up -d --build
2) docker-compose stop command -> docker-compose down

You can choose the name of the run application-name.properties (dev, stage, preprod) in spring boot
to do this, you must set the value of the variable SPRING_PROFILES_ACTIVE=name

Show container docker -> docker-compose ps
Stop docker container -> docker-compose down

show in container docker exec -it container_name bash

Show docker image -> docker images
Show logs container docker logs -f container name

Delete image -> docker rmi -f name_image
Delete all image -> docker rmi -f $(docker images -a -q)

Docker stop -> docker stop name_container
Docker delete container -> docker rm name_container

sudo service postgresql stop
sudo service postgresql start

