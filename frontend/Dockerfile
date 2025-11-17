# FROM nginx
FROM nginx:alpine3.22
RUN rm -rf /usr/share/nginx/html/index.html
COPY code /usr/share/nginx/html/index.html
CMD [ "nginx", "-g", "daemon off;" ]
