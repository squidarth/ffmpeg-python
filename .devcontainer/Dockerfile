# Use the official Python base image

FROM alpine:latest

RUN apk update &&     apk add ffmpeg &&     apk add --no-cache --virtual .build-deps gcc musl-dev &&     pip install ffmpeg-python &&     apk del .build-deps &&     rm -rf /var/cache/apk/*

    ENTRYPOINT ["python"]


    