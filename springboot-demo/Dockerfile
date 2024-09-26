# Step 1: Use a base image with JDK
FROM openjdk:17-jdk-alpine

# Step 2: Set the working directory inside the container
WORKDIR /app

# Step 3: Copy the Maven build output JAR file to the container
COPY target/springboot-demo-0.0.1-SNAPSHOT.jar app.jar

# Step 4: Expose the application port (default Spring Boot port)
EXPOSE 8080

# Step 5: Run the Spring Boot application
ENTRYPOINT ["java", "-jar", "app.jar"]
