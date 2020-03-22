FROM nginx:1.17.7-alpine

# Remove the default Nginx configuration
RUN rm /etc/nginx/conf.d/default.conf

# Add our Nginx config
COPY ./nginx.conf /etc/nginx/conf.d

# Copy our website content to the directory defined in our nginx.conf
COPY ./src /var/www/mysite

EXPOSE 8080
CMD ["nginx", "-g", "daemon off;"]
