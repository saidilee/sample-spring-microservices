# Use an official OpenJDK runtime as a parent image
FROM openjdk:8-jdk-alpine

# Set the maintainer label
LABEL maintainer="Piotr Minkowski <piotr.minkowski@gmail.com>"

# Add the application's jar to the container
ADD target/zipkin-service.jar zipkin-service.jar

# Make port 8080 available to the world outside this container
EXPOSE 9411

# Run the jar file
ENTRYPOINT ["java", "-jar", "/zipkin-service.jar"]
