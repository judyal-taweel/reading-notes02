# Spring RequestMapping

1.  @RequestMapping — by Path ---> @RequestMapping(value = "/ex/foos", method = POST)--> curl -i http://localhost:8080/spring-rest/ex/foos

2. @RequestMapping — the HTTP Method ---> @RequestMapping(value = "/ex/foos", method = POST)--> curl -i -X POST http://localhost:8080/spring-rest/ex/foos


###  RequestMapping and HTTP Headers

1. @RequestMapping With the headers Attribute
2. @RequestMapping Consumes and Produces
3. @RequestMapping Consumes and Produces

### RequestMapping With Path Variables

1. Single @PathVariable --->@PathVariable("id") long id)-->curl http://localhost:8080/spring-rest/ex/foos/1

2. Multiple @PathVariable ---> @PathVariable long fooid, @PathVariable long barid

3. @PathVariable With Regex--->Regular expressions can also be used when mapping the @PathVariable.

## Accessing Data with JPA
 JPA is a specification. It is a collection of classes and methods to persistently store the vast amounts of data into a database. It provides common prototype and functionality to ORM tools. By implementing the same specifiation, all ORM tools (like Hibernate, TopLink..) follows the common standarts.

 You can run the application from the command line with Gradle or Maven. You can also build a single executable JAR file that contains all the necessary dependencies, classes, and resources and run that. Building an executable jar makes it easy to ship, version, and deploy the service as an application throughout the development lifecycle, across different environments, and so forth.

![](imgs/JPA.png)

