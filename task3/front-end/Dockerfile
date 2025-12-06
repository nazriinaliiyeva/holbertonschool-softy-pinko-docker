# Use the latest Nginx image
FROM nginx:latest

# Copy static website content
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy Nginx configuration
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

