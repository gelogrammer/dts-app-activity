# Use the latest nginx image
FROM nginx:latest

# Copy the renamed HTML file to nginx web root as index.html (so it loads by default)
COPY netflix-index.html /usr/share/nginx/html/index.html

# Change Nginx config to listen on port 8085 instead of 80
RUN sed -i 's/listen 80;/listen 8085;/' /etc/nginx/conf.d/default.conf

# Expose ports 8085 and 3000
EXPOSE 8085
EXPOSE 3000

# Start Nginx (default command already set, but shown for clarity)
CMD ["nginx", "-g", "daemon off;"]