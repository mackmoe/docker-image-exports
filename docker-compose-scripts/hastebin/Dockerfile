FROM node:6-alpine

MAINTAINER Mo Nashington, mackmoe@3litedhome.net

RUN apk -U upgrade \
    && apk add git

ADD ./hastebin-server/  /app
WORKDIR /app
RUN npm install

ADD ./app.sh /app/
RUN chmod 755 app.sh

EXPOSE 3001

ENV STORAGE_TYPE file

CMD [ "./app.sh" ]
