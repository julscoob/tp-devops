FROM ubuntu:latest

RUN apk update && \
  apk add \
   nano \
   mongodb \
   nodejs && \
  mkdir /app

RUN npm install

COPY . /app

CMD cat /app/test.txt