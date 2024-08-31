# Use the latest version of Nginx as the base image
FROM nginx:latest

# Copy the Nginx configuration file to the appropriate directory
COPY proxy.conf /etc/nginx/conf.d/default.conf

# Expose port 80 to allow traffic to reach the Nginx server
EXPOSE 80
