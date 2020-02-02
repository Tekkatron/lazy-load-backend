FROM openjdk:8-alpine
MAINTAINER Andres Chavez (Tekka) <andres.chavez@sappturn.com>

WORKDIR /app

COPY ./build .
COPY ./application.yaml .

ENV DB_HOST=hostname \
    DB_PORT=7788 \
    DB_NAME=dbname \
    DB_USER=user \
    DB_PASS=secret

EXPOSE 9000


COPY ./launcher.sh .

RUN chmod +x launcher.sh

ENTRYPOINT ["./launcher.sh"]
