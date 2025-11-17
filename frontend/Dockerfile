FROM nginx
RUN rm -rf /usr/share/nginx/html/index.html
COPY code/ /usr/share/nginx/html/
CMD [ "nginx", "-g", "daemon off;" ]
