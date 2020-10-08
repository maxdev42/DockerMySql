- On pull l'image MySql depuis Docker Hub 
docker pull mysql/mysql-server:latest

- on vérifie qu'elle est bien téléchargée
docker images

- on run 
docker run --name=[container_name] -d mysql/mysql-server:latest

- on vérifie qu'elle est en cours d'exécution
docker ps

- On récupère le mot de passe de l'image depuis le fichier de logs 
docker logs XXX

- On se connecter 
docker exec -it XXX mysql -uroot -p

- On modifie le mdp 
mysql> ALTER USER 'root'@'localhost' IDENTIFIED BY '[newpassword]';
