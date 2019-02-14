FROM python:3.7-alpine

COPY requirements.txt  /app

WORKDIR /app
RUN apk add --no-cache --virtual .build-deps gcc musl-dev
RUN pip3 install -r requirements.txt
RUN apk del .build-deps gcc musl-dev

