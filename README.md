# mysql-phpmyadmin-docker
Docker composer repository to MariaDB and PHPMyAdmin with data persistence on local folder

#Instructions
This little file docker-composer.yml creates 2 containers. One to host mysql/mariadb server on port 3306, and other to expose an PHPMySQL application to Database administration.

To run this docker compose you myst have:
- Docker machine installled
- Docker composer installed

To run docker compose use:
  docker-compose up -d
  
To kill the dockers containers:
  docker-compose down

#Important notes
- use http://localhost:8081 to access PHPMyAdmin
- On server use: db (yes, just db for server/host)
- user: root
- password: password
- in you application use as Mysql Host: localhost
- use as MySQL port: 3306
- DATA PERSISTANCE: this docker-compose will persist the data on "db_persist" folder as a mysql files structure.


