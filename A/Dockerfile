FROM ubuntu:latest

RUN apt-get update && \
  apt-get install \
   nano \
   mongodb \
   nodejs && \
  mkdir /app

RUN npm install

COPY . /app

CMD cat /app/test.txt