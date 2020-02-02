FROM openjdk:8-alpine
MAINTAINER Andres Chavez (Tekka) <andres.chavez@sappturn.com>

WORKDIR /app

COPY . .



CMD [ "java -jar build/libs/lazy-load-app-1.0.jar --spring.config.location=./application.yaml" ]
