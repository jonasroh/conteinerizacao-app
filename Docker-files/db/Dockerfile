FROM mysql:5.7.25

LABEL "Project"="java_app"

ENV MYSQL_ROOT_PASSWORD="dbpass"
ENV MYSQL_DATABASE="db_app"

ADD db_backup.sql docker-entrypoint-initdb.d/db_backup.sql
