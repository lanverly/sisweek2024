FROM nginx:latest
LABEL Author="Byron Lanverly"

ENV APP_HOME /var/www/html

COPY ./site /var/www/html
COPY default.conf /etc/nginx/conf.d/default.conf

RUN chmod 755 -R /var/www/html

EXPOSE 80

ENTRYPOINT [ "nginx" ]
CMD ["-g", "daemon off;"]