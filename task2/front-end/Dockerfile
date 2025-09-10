FROM nginx:latest

WORKDIR /var/www/html/softy-pinko-front-end

COPY ./softy-pinko-front-end/assets/ /var/www/html/softy-pinko-front-end/assets/

COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

COPY ./softy-pinko-front-end/index.html /var/www/html/softy-pinko-front-end
