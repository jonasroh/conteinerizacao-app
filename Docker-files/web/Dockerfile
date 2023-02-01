FROM nginx
LABEL "Project"="java_app"

RUN rm -rf /etc/nginx/conf.d/default.conf
COPY nginxapp.conf /etc/nginx/conf.d/java_app.conf