FROM alpine:latest
RUN apk add --no-cache openjdk17
WORKDIR /app
COPY ./Docker-1/target/demo-0.0.1-SNAPSHOT.jar .
EXPOSE 8080
CMD ["java", "-jar", "demo-0.0.1-SNAPSHOT.jar"]