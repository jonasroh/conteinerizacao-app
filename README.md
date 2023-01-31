# conteinerizacao-app-
Contaneirização de um projeto Java usando Docker

PASSOS
- Encontra uma imagem do dockerhub
- Escrever um dockerfile para customizar imagens
- Escrever um docker-compose.yml file para executar container múltiplos
- Testar e hostear as imagens no dockerhub


//////////// verificar isso /////////////
## Prerequisites
- JDK 1.8 or later
- Maven 3 or later
- MySQL 5.6 or later
######
## Technologies 
- Spring MVC
- Spring Security
- Spring Data JPA
- Maven
- JSP
- MySQL
## Database
Here,we used Mysql DB 
MSQL DB Installation Steps for Linux ubuntu 14.04:
- $ sudo apt-get update
- $ sudo apt-get install mysql-server

Then look for the file :
- /src/main/resources/accountsdb
- accountsdb.sql file is a mysql dump file.we have to import this dump to mysql db server
- > mysql -u <user_name> -p accounts < accountsdb.sql

////////////////////////////////////////

TOMCAT DOCKERFILE
A versão da imagem escolhida é uma compatível com a aplicação.
No arquivo Dockerfile é removido a aplicação Default da imagem através do comando RUN. O COPY é utilizado para copiar o build da aplicação. Por fim,  binário "catalina.sh" é executado para rodar o tomcat.
A aplicação será exposta na porta 8080.

MYSQL DOCKERFILE
A imagem utililizada foi uma compatível com a aplicação. Duas variáveis foram setadas para definir a senha do user ROOT e também o nome do banco de dados.
A estrutura do banco de dados será criado baseado no arquivo SQL copiado para o dir /docker-entrypoint-initdb.d
Esse diretório é o indicado na documentação da imagem.

NGINX DOCKERFILE
A imagem utilizada foi a latest. O arquivo de configuração default foi removido e substituído por outro.