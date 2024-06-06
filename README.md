# Swagger Integration
To integrate Swagger on a Java Spring Boot application you need to paste the following dependencies in the `pom.xml` file:
```
<dependency>
    <groupId>org.springdoc</groupId>
    <artifactId>springdoc-openapi-starter-webmvc-ui</artifactId>
    <version>2.3.0</version>
</dependency>
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-validation</artifactId>
</dependency>
```
In certain environments the swagger will appear just by the insertion of the dependencies, but won't in others.
To make it appear regardless of the environment you need to set the following properties in the `application.properties` file:
```
#SWAGGER
springdoc.swagger-ui.enabled=true
springdoc.api-docs.enabled=true
```
The Swagger will be available at `http://localhost:{be-port-number}/swagger-ui.html`
