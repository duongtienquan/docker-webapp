FROM ubuntu:16.04

WORKDIR /root/

# apt update -y
RUN apt update -y

# apt install curl -y
RUN apt install curl -y

# curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash

# apt install -y nodejs
RUN apt install -y nodejs

#copy code to container
COPY . /root/

# npm install
RUN npm install

EXPOSE 8000

# FRONT_URL=<http://ip-frontend:port> npm start
CMD FRONT_URL=${FRONT_URL} npm start

