# Sanic Base App Dockerfile

This image is meant to be a starting point for you to build your own [Sanic](https://github.com/huge-success/sanic) application running on Docker. It is a "base" app in that it makes no decisions for you and is completely unopinionated.

Are you looking for a **best practices** solution with some guidance on how to setup your Sanic App? We will be releasing a second image in the future with some more guidance.

## What does this image do?

It preinstalls the latest [**Sanic LTS**](https://sanic.readthedocs.io/en/18.12.0/) version on top of a **Python 3.7**. The container runs Alpine Linux.

## How do I use this?

Setup your own Dockerfile

    FROM sanicframework/sanic:LTS

    RUN mkdir /srv
    COPY . /srv

    EXPOSE 8888

    ENTRYPOINT ["python3" "/srv/my-sanic-server.py"]

Build it

    docker build -t my-sanic-server .

Run it as you would any other container

    docker run my-sanic-server
