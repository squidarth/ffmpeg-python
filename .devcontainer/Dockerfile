# Use the official Python base image

FROM alpine:latest

RUN apk update &&     apk add ffmpeg &&     apk add --no-cache --virtual .build-deps gcc musl-dev python3-dev libffi-dev openssl-dev &&     wget https://bootstrap.pypa.io/get-pip.py &&     python3 get-pip.py &&     pip install ffmpeg-python &&     apk del .build-deps &&     rm -rf /var/cache/apk/*

    