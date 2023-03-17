FROM openjdk:19
VOLUME /tmp
ARG JAR_FILE
COPY PubSub-Service-0.0.1-SNAPSHOT.jar app.jar
COPY application.properties application.properties
ENTRYPOINT ["java","-jar","/app.jar", "--spring.config.location=application.properties"]