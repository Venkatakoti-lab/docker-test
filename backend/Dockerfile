# FROM node:20
FROM node:20.19.5-alpine3.22
WORKDIR /opt/backend
COPY package.json ./
COPY *.js ./
RUN npm install
ENV DB_HOST="mysql"
#systemctl will not work in containers
CMD ["node", "index.js"]