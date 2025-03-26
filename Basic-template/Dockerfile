# Use the official Nginx image
FROM nginx:latest

# Copy your Nginx configuration file
COPY ./nginx.conf /etc/nginx/nginx.conf

# Expose the port Nginx listens on (default is 80)
EXPOSE 80

# Command to start Nginx
CMD ["nginx", "-g", "daemon off;"]