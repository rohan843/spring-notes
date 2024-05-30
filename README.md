# Spring Notes

## Contents

- [Spring Notes](#spring-notes)
  - [Contents](#contents)
  - [Basic Background](#basic-background)

## Basic Background

**Spring** is a popular framework for building java applications. It provides us with multiple helper classes and annotations.

However, there is an issue with Spring that it is too complex to setup a project in it. This is where **Spring Boot** is useful. It eases the initial configuration before Spring development. It minimizes the amount of manual configuration required and also performs auto-configuration based on props file and JAR classpath. It helps to resolve dependency conflicts (such as Maven or Gradle) and provides an embedded HTTP server that supports Tomcat, Jetty, Undertow, etc.

We can think of Spring Boot as a simplification layer above Spring. It still uses Spring behind the scenes and acts as an abstraction.

Spring Boot provides an application called the **Spring Initializr** that allows us to quickly create a Spring Boot project. We can access it at the website: [https://start.spring.io](https://start.spring.io). This creates a Maven/Gradle project that can then be imported into any IDE or used manually from a text editor.

For portability purposes, Spring Boot provides us with an embedded HTTP server in any JAR. This server can be Tomcat, Jetty, Undertow, etc. This allows us to run our application in a standalone fashion without the need for a separate installation. This process is as simple as:

```bash
java -jar path/to/jar/file.jar
```

In case we do not wish for an embedded server, we can also create WAR files (Web Application aRchive) and deploy them to an external server.
