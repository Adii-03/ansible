# Start with a base image containing Java runtime (JDK 11 & Maven 3.6.3)
FROM maven:3.6.3-openjdk-11

# The application's .jar file
ARG JAR_FILE=target/*.jar

# Add the application's .jar to the container
ADD ${JAR_FILE} app.jar

# Run the jar file 
ENTRYPOINT ["java","-jar","/app.jar"]
