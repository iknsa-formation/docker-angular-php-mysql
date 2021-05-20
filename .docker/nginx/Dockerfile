FROM nginx

RUN rm /etc/nginx/conf.d/default.conf
COPY .docker/nginx/my.conf /etc/nginx/nginx.conf

WORKDIR /usr/share/nginx/html
RUN chmod -R 755 /usr/share/nginx/html

ENTRYPOINT ["nginx", "-g", "daemon off;"]