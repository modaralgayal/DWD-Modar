FROM ubuntu:latest

RUN apt-get update && apt-get install -y nodejs

RUN apt-get install -y curl

RUN apt-get install -y npm

RUN curl -sL https://deb.nodesource.com/setup_16.x | bash -

RUN npm install -g serve

COPY . .

EXPOSE 5001

CMD [ "serve", "-s", "-l", "5001", "build" ]