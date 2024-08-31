# Use the latest Nginx image
FROM nginx:latest

# Remove the default configuration file
RUN rm /etc/nginx/conf.d/default.conf

# Copy custom Nginx configuration
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Copy front-end files to the Nginx default directory
COPY softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Expose port 9000
EXPOSE 9000
