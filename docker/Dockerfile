FROM alpine:3.12

ARG VERSION

RUN apk update && \
    apk add py3-pip

ADD https://raw.githubusercontent.com/opendatapedia/opendatapedia/main/requirements.txt /tmp/requirements.txt

RUN pip3 install -r /tmp/requirements.txt

LABEL opendatapedia.alpine.version=3.12 \
      opendatapedia.python.version=3.8.5 \
      opendatapedia.app.version=${VERSION}