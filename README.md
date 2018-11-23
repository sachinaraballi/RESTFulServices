# RESTFulServices
RESTFul Services in Java using Jersey

## Introduction 

### What is Jersey 

[Jersey](https://jersey.github.io/) RESTful Web Services framework is open source, production quality,
framework for developing RESTful Web Services in Java that provides support 
for JAX-RS APIs and serves as a JAX-RS (JSR 311 & JSR 339) Reference Implementation.

Jersey framework is more than the JAX-RS Reference Implementation. Jersey provides 
it’s own API that extend the JAX-RS toolkit with additional features and 
utilities to further simplify RESTful service and client development

### What is JAX-RS API
Java™ API for RESTful Web Services (JAX-RS) delivers API for RESTful Web Services development in Java SE and Java EE.

### Hands on 

#### 1.1. Creating a New Jersey Project from Maven Archetype and Grizzly Server 

Install Apache Maven and add folder to system path and execute the following command in terminal

```maven
mvn archetype:generate -DarchetypeArtifactId=jersey-quickstart-grizzly2 
-DarchetypeGroupId=org.glassfish.jersey.archetypes -DinteractiveMode=false 
-DgroupId=com.example -DartifactId=simple-service -Dpackage=com.example
-DarchetypeVersion=2.27
```

If you get any proxy issues 
Add proxies to maven/conf/settings.xml 
and .m2/settings.xml 


simple-service will be generated. 
Go to src folder where pom.xml is located 
run commands
```maven
mvn clean test (compiles and builds the project)
mvn exec:java (starts the grizzy server and deploys) 
```

then run curl command 
$ curl http://localhost:8080/myapp/myresource

Got it!

The main Java Annotations are : 

@Path - resource location

@GET - Type of request

@Produces - Output format





