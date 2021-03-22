# mysql-phpmyadmin-docker PT_BR
Este é um arquivo de docker compose para rodar MariaDB (Mysql) e PHPMyAdmin com persistências de dados na pasta local.
Sua função é permitir o desenvolvimento de aplicações sem a necessidade de instalar localmente instancias do Mysql nem PHP na estação de desenvolvimento.

#Instructions
Este pequeno arquivo docker-composer.yml cria 2 containes. Um para hospedar o mysql/mariadb na porta 3306 e outro para expor um PhpMyadmin para administrar suas bases.

Para rodar este docker você precisa:
- Docker machine instalado
- Docker composer instalado

Para rodar e criar os containers rode no terminal:
  docker-compose up -d
  
Para matar os containers:
  docker-compose down

#Notas Importantes
- use http://localhost:8081 para acessar o PhpMyAdmin
- Na tela do PhpMyAdmin no campo servidor/host use simplesmente: db
- user: root
- password: password
- na sua aplicação coloque como servidor de banco de dados: localhost
- a porta do Mysql exposta é: 3306
- PERSISTÊNCIA DE DADOS: este docker-compose faz a persistência de dados na pasta "db_persist" na raiz do projeto.




# mysql-phpmyadmin-docker EN_US
Docker composer repository to MariaDB and PHPMyAdmin with data persistence on local folder

#Instructions
This little file docker-composer.yml creates 2 containers. One to host mysql/mariadb server on port 3306, and other to expose an PHPMySQL application to Database administration.

To run this docker compose you myst have:
- Docker machine installled
- Docker composer installed

To run docker compose use in terminal:
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


