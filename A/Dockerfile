FROM ubuntu:latest

RUN apt-get update -y && \
  apt-get install -y \
   nano \
   mongodb \
   nodejs \
   nodejs-legacy \
   npm && \
  mkdir /app

RUN npm install

COPY . /app

CMD cat /app/test.txt