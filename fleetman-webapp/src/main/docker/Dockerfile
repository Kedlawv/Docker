FROM openjdk:8u131-jdk-alpine

MAINTAINER "com.wabu"

WORKDIR /usr/local/bin/

COPY maven/target/fleetman-0.0.1-SNAPSHOT.jar webapp.jar

EXPOSE 8080

CMD ["java","-Dspring.profiles.active=docker-demo","-jar","webapp.jar"]