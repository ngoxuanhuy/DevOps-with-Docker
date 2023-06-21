FROM openjdk:8

WORKDIR /spring-project

COPY . .

RUN chmod 700 mvnw && ./mvnw package

ENTRYPOINT ["java", "-jar", "./target/docker-sample-1.1.3.jar"]