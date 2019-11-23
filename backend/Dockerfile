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

EXPOSE 8000

# FRONT_URL=<http://ip-frontend:port> npm start
CMD $(FRONT=URL) npm start

