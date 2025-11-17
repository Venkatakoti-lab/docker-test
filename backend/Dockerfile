# FROM node:20
FROM node:20.19.5-alpine3.22
RUN addgroup -S expense && adduser -S expense -G expense
RUN mkdir /opt/backend
RUN chown -R expense:expense /opt/backend
WORKDIR /opt/backend
COPY package.json ./
COPY *.js ./
RUN npm install
ENV DB_HOST="mysql"
USER expense
#systemctl will not work in containers
CMD ["node", "index.js"]