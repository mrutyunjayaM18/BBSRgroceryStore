# Stage 1: Use a lightweight Nginx image to serve the static files
FROM nginx:alpine

# Remove the default Nginx welcome page
RUN rm /usr/share/nginx/html/index.html

# Copy your application's single HTML file into the Nginx web root directory
COPY index.html /usr/share/nginx/html/

# Expose port 80, which is the default port for Nginx
EXPOSE 80

# The default command for the nginx image is to start the server.
# This line ensures it runs in the foreground.
CMD ["nginx", "-g", "daemon off;"]
