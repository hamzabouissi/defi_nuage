FROM openjdk:8-jdk-alpine
RUN addgroup -S spring && adduser -S spring -G spring
EXPOSE 8000
USER spring:spring
COPY target/spring-boot-docker.jar spring-boot-docker.jar
ENTRYPOINT ["java","-jar","/spring-boot-docker.jar"]