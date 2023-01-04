# 15 Spring Boot Best Practices to create Production grade microservices

### 1. Spring initializer 
- https://start.spring.io/
  - Why use tools? - so we are getting the same version and we are following the same best practices
- If we add dependencies manually on pom.xml, we might end up adding older version when we copy paste from some other sources
- Use all dependencies with cleaner configuration right out of the box


### 2. Open API Specification (formerly Swagger)
- Swagger 3.0 is called Open API Specification
- Swagger hub as files where you can post open api specifications, and generate code out of it
- You can leverage different maven plugins for this
- Leverage these so you get standardized code without coding it manually


### 3. Auto Configurations
- Lets spring boot know what it needs when the application starts up 
- Helps with boot up time
- Configures your spring application so that it can serve you better when there are some configuration or dependency specific tasks


### 4. Constructor Injection
- Use constructor injection instead of @Autowired annotation. 
- Using constructor injection create a best code practice
- Using @Autowired may end up creating a lot of spring specific dependencies (+ a bloated class)
- Leverage Spring Autowiring out of the box instead of using @Autowired annotation 


### 5. Modular packages (creating modular code) 
- Controllers in controllers folder, services in services folder, etc.
- Create feature specific folders, based on your requirement 
- Easier to navigate the code


### 6. Using Data Transfer Objects (DTO)
- Helps you to create a structure to the response or the objects which you use within the spring boot application 
- Helps you create standards


### 7. Leverage Bean Validations (@NotBlank annotation) 
- Validation annotations can be added to your Data Transfer Objects
- Don’t really need to have custom validation in your code
- Most of the time when you are exposing APIs, you are vulnerable to some data which could create issues 


### 8.Externalize Configuration (Inject at Runtime) 
- dev or prod environment specific configurations,  
- Can be injected dynamically or injected from external source 
- Externalize source if possible 


### 9. Logging Stanarization Configuration
Help you in navigating through your logs
Use same log format across all microservices, or it will create confusions
ex) log4j


### 10. Exposing your healthcheck endpoints
- Help platform to assess what’s happening to your application, and it might restart your application when it requires (ex. kubernetes has feature to stream liveness)


### 11. Exception Handlers
- Using a common or a framework level exception
- Use interceptors to identify the issues, log them, and translate them into meaningful information
return a proper error response to client, so we don’t have to expose the error that is happening within the application 


### 12. Testing by Isolation (cucumber/spec)
- Always test your application by isolating your flow or else testing is going to be huge
- Create test individually for integrating all your modules within the same application and test only those
- Automate test as part of your CI/CD pipeline, so that you get to know the feedbacks whenever you’re committing your code


### 13. Avoid adding extra dependencies
- Already a lot of jars inside the supreme boot application, which can slow down the start up process
- Higher risk for dependency issues
- Make sure you know why you’re adding those dependencies

### 14. Faster boot up
- Leverage lazy initialization - load your classes whenever a request comes in or whenever your flow is getting triggered
- Leverage Spring native library (recently launched) 


### 15. Reactive programming
- Leverage reactive calls whenever required, so that you can have productive usage of your threads, and you can get callbacks whenever you need to process messages from the external source
- Help application speed - you might not be idle in terms of waiting for io operations, doing dependency cals, reading files, etc.
