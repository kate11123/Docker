FROM nginx

RUN mkdir -p /var/www/backend/html
RUN chown -R $USER:$USER /var/www/backend/html
RUN chown -R 755 /var/www/backend
RUN rm /etc/nginx/conf.d/default.conf

COPY backend.json /var/www/backend/html/
COPY backend.conf /etc/nginx/conf.d/
