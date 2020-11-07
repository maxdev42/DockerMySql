- Downloading the MySql image from Docker Hub
docker pull mysql/mysql-server:latest

- Checking that the image is correctly downloaded
docker images

- Running container with our image
docker run --name=[container_name] -d mysql/mysql-server:latest

- Checking that the container is online
docker ps

- Recovering the image password from the logs file
docker logs XXX

- Connection to MySql on our container
docker exec -it XXX mysql -uroot -p

- Modification of MySql password
mysql> ALTER USER 'root'@'localhost' IDENTIFIED BY '[newpassword]';
