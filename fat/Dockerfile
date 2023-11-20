# Use a base image with Java already installed
FROM openjdk:11-jre-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the Maven project files to the container
COPY . /app

# Build the Maven project inside the container
RUN mvn clean install

# Define the command to run your Java application
CMD ["java", "-jar", "target/your-application.jar"]
