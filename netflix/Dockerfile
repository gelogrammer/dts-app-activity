FROM nginx:latest
COPY index.html /usr/share/nginx/html/index.html
RUN sed -i 's/listen 80;/listen 8085;/' /etc/nginx/conf.d/default.conf
EXPOSE 8085
EXPOSE 3000
CMD ["nginx", "-g", "daemon off;"]