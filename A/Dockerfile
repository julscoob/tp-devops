FROM ubuntu:latest

RUN apt-get update -y && \
  apt-get install -y \
   nano \
   mongodb \
   nodejs && \
  mkdir /app

RUN npm install

COPY . /app

CMD cat /app/test.txt