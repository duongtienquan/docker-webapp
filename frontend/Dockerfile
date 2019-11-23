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

# API_URL=<http:/ip-backend:port> npm start
CMD API_URL=${API_URL} npm start
