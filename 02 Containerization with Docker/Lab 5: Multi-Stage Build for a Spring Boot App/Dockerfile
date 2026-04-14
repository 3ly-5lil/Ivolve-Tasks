FROM maven:3.9.14-eclipse-temurin-17-alpine
WORKDIR /app
COPY Docker-1/ .
RUN mvn clean package

FROM eclipse-temurin:17-jdk-alpine
WORKDIR /app
COPY --from=0 /app/target/demo-0.0.1-SNAPSHOT.jar .
EXPOSE 8080
CMD ["java", "-jar", "demo-0.0.1-SNAPSHOT.jar"]