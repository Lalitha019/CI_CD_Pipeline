# Build stage - Maven runs inside Docker
FROM maven:3.9-eclipse-temurin-11 AS build

WORKDIR /app

COPY pom.xml .
COPY src ./src

RUN mvn clean package -DskipTests

#Runtime stage
FROM adoptopenjdk/openjdk11:alpine-jre

WORKDIR /opt/app

COPY --from=build /app/target/*.jar app.jar

ENTRYPOINT ["java","-jar","app.jar"]
