FROM tomcat:8.5.47-jdk8-openjdk

MAINTAINER "com.wabu"

RUN rm -rf /usr/local/tomcat/webapps/*

COPY ./target/fleetman-0.0.1-SNAPSHOT /usr/local/tomcat/webapps/ROOT.war

ENV JAVA_OPTS="-Dspring.profiles.active=docker-demo"

EXPOSE 8080

CMD ["catalina.sh","run"]