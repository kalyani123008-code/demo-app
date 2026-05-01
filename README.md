# Demo App

A simple Maven project demonstrating CI/CD with Jenkins and GitHub.

## Project Structure

- `src/main/java/com/example/App.java` - Main application class
- `src/test/java/com/example/AppTest.java` - Unit tests
- `pom.xml` - Maven configuration
- `Jenkinsfile` - Jenkins pipeline for CI/CD

## Build

To build the project locally:

```bash
mvn clean compile
mvn test
mvn package
```

## Jenkins Setup

1. Ensure Jenkins has Maven installed and configured.
2. Create a new pipeline job in Jenkins.
3. Set the pipeline script from SCM, pointing to this repository's Jenkinsfile.
4. Run the job to build, test, and package the application.

## GitHub Integration

Push this code to a GitHub repository. The Jenkinsfile is configured to checkout from GitHub.