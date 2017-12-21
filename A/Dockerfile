
FROM node:alpine

RUN apk update && \
  apk add \
   nano \
   mongodb \
   nodejs && \
   mkdir /app \
   mkdir /src
WORKDIR /src
ADD app/package.json /src/package.json
ADD app/package-lock.json /src/package-lock/json
RUN npm install

COPY . /app

CMD cat /app/test.txt