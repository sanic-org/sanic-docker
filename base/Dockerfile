FROM python:alpine3.8

RUN apk update \
    && apk add build-base

RUN mkdir /usr/src/app

COPY ./requirements.txt /usr/src/app/requirements.txt

WORKDIR /usr/src/app
ENV PYTHONPATH /usr/src/app

RUN pip3 install -r requirements.txt
