# Start with a base image containing Java runtime (JDK 11 & Maven 3.6.3)
FROM maven:3.6.3-openjdk-11

# Copy the application's .jar to the container
COPY target/*.jar app.jar

# Run the jar file, this will only run when we start the container
ENTRYPOINT ["java","-jar","/app.jar"]
