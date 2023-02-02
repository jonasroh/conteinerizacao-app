
# Introdução
Nesse projeto foi realizado a conteinerização de uma aplicação já existente. A conteinerização é uma tecnologia para empacotar e implantar aplicativos em um ambiente leve e isolado. Os contêineres fornecem um ambiente consistente para o aplicativo, facilitando a implantação e a execução em difrentes sistemas e infraestruturas.

A aplicação se trata de um website e esse aplicativo web é uma rede social escrito por desenvolvedores em linguagem java. 

# Serviços
Os serviços utilizados para subir essa aplicação são:
- Nginx
  O nginx é usado para criar a experiência de um load balancer.

- Tomcat
  Todo o tráfego que chega ao nginx é direcionado ao Tomcat. O Apache Tomcat é um serviço de aplicação web Java. O Tomcat é um famoso serviços para hostear aplicações escritas em Java.

- RabbitQM
  O RabbitMQ funciona como uma intermediário para mensagens, mas para esse projeto esse serviço não é funcional. Ele se encontra presente só para aumentar o grau de complexidade do projeto.

- Mysql
  O MySQL é o banco onde está armezado as informações de usuários.

- Memchached
  O memcached é um sistema de cache em memória. Após um primeiro acesso, os dados dos usuários são armazenados no memcached afim de acelerar as querys.