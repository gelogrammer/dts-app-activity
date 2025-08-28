# Use the latest nginx image
FROM nginx:latest

# Copy your HTML file to the default nginx web directory
COPY index.html /usr/share/nginx/html/index.html

# Optional: Customize nginx to listen on a different port (e.g., 8085)
# Only if you need it — otherwise, keep default port 80
RUN sed -i 's/listen 80;/listen 8085;/' /etc/nginx/conf.d/default.conf

# Document that the container listens on port 8085
EXPOSE 8085

# Nginx will start automatically with the default command
# CMD ["nginx", "-g", "daemon off;"] ← already set in nginx image