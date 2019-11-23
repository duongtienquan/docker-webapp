FROM ubuntu:16.04

# apt update -y
RUN apt update -y
# apt install curl -y
RUN apt install curl -y
# curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
# apt install -y nodejs
RUN apt intall -y nodejs
# npm install
npm install

EXPOSE 5000

# API_URL=<http://ip-backend:port> npm start
CMD $(API_URL) npm start
