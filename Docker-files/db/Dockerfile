FROM mysql:5.7.25

ENV MYSQL_ROOT_PASSWORD="dbpass"
ENV MYSQL_DATABASE="bancoDeDados"

ADD db_backup.sql /docker-entrypoint-initdb.d/db_backup.sql