#  Task: Create a Simple REST API with Spring Boot  

##  Objective  
Build a basic Spring Boot REST API that returns a simple message when accessed.  

##  Instructions  

1. Create a Controller Class  
   - Inside `src/main/java/com/example/demo/`, create a new file `HelloController.java`.  
   - Example Code:  

   ```java
   package com.example.demo;

   import org.springframework.web.bind.annotation.GetMapping;
   import org.springframework.web.bind.annotation.RequestMapping;
   import org.springframework.web.bind.annotation.RestController;
   
   @RestController
   @RequestMapping("/api")
   public class HelloController {

       @GetMapping("/hello")
       public String sayHello() {
           return "Hello, Spring Boot!";
       }
   }
```
2. Run the Spring Boot Application  
- Start the application.  

3. Test the API : Open a browser or Postman and visit:  

```bash
   http://localhost:8080/api/hello
```