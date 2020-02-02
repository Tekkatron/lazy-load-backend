FROM openjdk:8-alpine
MAINTAINER Andres Chavez (Tekka) <andres.chavez@sappturn.com>

WORKDIR /app

COPY ./build .

ENV DB_HOST ""
ENV DB_PORT ""
ENV DB_NAME ""
ENV DB_USER ""
ENV DB_PASS ""

EXPOSE 9000

CMD [ "java -jar build/libs/lazy-load-app-1.0.jar --spring.config.location=./application.yaml" ]
