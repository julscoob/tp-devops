
FROM ubuntu:latest

RUN apt-get update -y && \
  apt-get install -y \
   nano \
   mongodb \
   nodejs \
   nodejs-legacy \
   npm && \
  mkdir /app

WORKDIR /src
ADD app/package.json /src/package.json
ADD app/package-lock.json /src/package-lock/json
RUN npm install

COPY . /app

CMD cat /app/test.txt
