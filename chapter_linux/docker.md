


systemctl start docker
systemctl stop docker
systemctl status docker

docker search <image.name, ex: centos, tomcat >

docker images
docker rmi -f <image.name>

docker ps
docker stop <image.id | image.name>
docker stop $(docker ps -a)			stop all


docker run -dp 8001:8080 tomcat	8001 is asscess port

docker exec -it <name | contrainter.id> /bin/bash

docker cp xxx.xx <contaniner.anme>:/<path>

docker build -t <name> .

