FROM openjdk:18-alpine
RUN addgroup -S spring && adduser -S spring -G spring
VOLUME ["/TEMP"]
USER spring:spring
COPY target/*.jar app.jar
ARG JAR_FILE=target/department-service-0.0.1-SNAPSHOT.jar

ENTRYPOINT ["java","-jar","/app.jar"]


COPY target/*.jar app.jar