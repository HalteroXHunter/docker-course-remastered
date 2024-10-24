## 1. Which base image do you want to use?
FROM maven:3.8-openjdk-17-slim
## 2. Set the working directory.
WORKDIR /app/
## 3. Copy the application's project files into the working directory.
COPY springboot-demo/ .
## 4. install dependencies listed inside the pom.xml file.
RUN mvn package
## 5. Document and inform the developer that the application will use the container port: 8080.
EXPOSE 8080
## 6. Define the command to run when the container starts.
CMD ["java", "-jar", "target/demo-0.0.1-SNAPSHOT.jar"]