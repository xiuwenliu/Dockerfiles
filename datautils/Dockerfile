FROM python:3.7

COPY ./requirements.txt  /

WORKDIR /
RUN apk add --no-cache --virtual .build-deps gcc musl-dev
RUN pip3 install -r requirements.txt
RUN apk del .build-deps gcc musl-dev

