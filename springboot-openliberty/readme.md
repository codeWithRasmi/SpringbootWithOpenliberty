# Getting Started

### Reference Documentation
For further reference, please consider the following sections:

* [Official Gradle documentation](https://docs.gradle.org)
* [Spring Boot Gradle Plugin Reference Guide](https://docs.spring.io/spring-boot/4.0.0/gradle-plugin)
* [Create an OCI image](https://docs.spring.io/spring-boot/4.0.0/gradle-plugin/packaging-oci-image.html)
* [Spring Web](https://docs.spring.io/spring-boot/4.0.0/reference/web/servlet.html)
* [Spring Boot DevTools](https://docs.spring.io/spring-boot/4.0.0/reference/using/devtools.html)
* [Docker Compose Support](https://docs.spring.io/spring-boot/4.0.0/reference/features/dev-services.html#features.dev-services.docker-compose)
* [Spring Data JPA](https://docs.spring.io/spring-boot/4.0.0/reference/data/sql.html#data.sql.jpa-and-spring-data)

### Local Development Mode Guides
The following guides illustrate how to run the application in Local Development Mode:

* User gradle build to build and run the application
* Modify server.xml inside src/deployment folder to configure the application server
* Download and install Open Liberty from https://openliberty.io/downloads/
* Create a server using the Liberty `server create <server-name>` command
* We have created a task to copy the deployment files to the **dropins** folder. Update your openLiberty installation path, then run the following command:
  ```
  ./gradlew deployToLiberty
  ```
* Goto to the openLiberty server's bin folder and run the server:
  ```
  ./server run <server-name>
  ```
* You can see the application running at `http://localhost:9080/app`

