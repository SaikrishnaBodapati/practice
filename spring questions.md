**Spring Question**



* What is Spring MVC?



* Difference between @Controller and @RestController



* What is @RequestMapping?



* Difference between @GetMapping and @PostMapping



* What is JPA?



* What is Hibernate?



* What is Entity?



* What is JpaRepository?



* why do we use application.properties and application.yml what is the use and which is better?



* What problem does Lombok solve?



* What does @Data include?



* what is @Request body



* what is @Request param



* what is @PathVariable ?



#### IoC (Inversion of Control)





* What is Inversion of Control (IoC)?



* Why is IoC important in Spring?



* How does Spring implement IoC?



* What problem does IoC solve?



* What is the difference between IoC and Dependency Injection?



* What is the IoC container?



* How does Spring manage objects using IoC?



* What are the advantages of IoC?



#### Dependency Injection (DI



* What is Dependency Injection?



* Why is Dependency Injection important?



* What are the types of Dependency Injection?



* What is Constructor Injection?



* What is Setter Injection?



* What is Field Injection?



* Why is constructor injection recommended?



* What happens if multiple beans of the same type exist?



* How does Spring resolve dependency conflicts?



* What is @Autowired?



* What is @Qualifier?



#### Spring Bean



* What is a Spring Bean?



* How are beans created in Spring?



* What are the scopes of a bean?



* What is the difference between singleton and prototype beans?



* How does Spring manage bean objects?



* How can you define a bean manually?



* What is @Bean annotation?



* What is the difference between @Component and @Bean?



#### Spring Container



* What is a Spring Container?



* What are the responsibilities of the Spring container?



* What are the types of Spring containers?



* What is the difference between BeanFactory and ApplicationContext?



* Why does Spring Boot use ApplicationContext?



* What happens inside the container during application startup?



* How does the container manage dependencies?



##### Component Scanning



* What is component scanning?



* What annotations are detected during component scanning?



* What is @ComponentScan?



* How does Spring Boot automatically scan components?



* What happens if a component is outside the scanned package?



* How can you customize package scanning?



##### Autowiring



* What is Autowiring?



* What does @Autowired do?



* What are the modes of autowiring?



* What happens if multiple beans exist?



* What is @Qualifier used for?



* What is @Primary?



* What happens if a dependency is not found?



##### Bean Lifecycle



* What is the lifecycle of a Spring bean?



* What are the phases of bean lifecycle?



* What is @PostConstruct?



* What is @PreDestroy?



* When are lifecycle methods executed?



* How does Spring destroy beans?



* What happens during bean initialization?



* Typical lifecycle flow:
1. Bean Creation
2. Dependency Injection
3. @PostConstruct
4. Bean Ready
5. @PreDestroy
6. Configuration Classes



* What is a configuration class?



* What does @Configuration do?



* What is the difference between @Configuration and @Component?



* What is @Bean?



* Why use Java configuration instead of XML?



* How are configuration classes processed by Spring?







##### Stage 2 – Spring Boot Basics



* Spring Boot Architecture



* What is Spring Boot architecture?



* What are the main layers in Spring Boot?



* What is the role of controller layer?



* What is the service layer?



* What is the repository layer?



* What is the entity layer?



* What is DTO in Spring Boot?



* How does a request flow through Spring Boot?



* Typical architecture:



* Controller → Service → Repository → Database





#### Spring Boot Starter Dependencies

* Why are starters used?



* What does spring-boot-starter-web include?



* What does spring-boot-starter-data-jpa include?



* What is the advantage of starters?



* How do starters simplify dependency management?



* Spring Boot Auto Configuration



* What is auto configuration?



* How does Spring Boot perform auto configuration?



* What is @EnableAutoConfiguration?



* What is @SpringBootApplication?



* What files are used internally for auto configuration?



* How does Spring Boot decide which configuration to load?

##### 

##### application.properties / application.yml



* What is application.properties?



* What is application.yml?



* What is the difference between properties and YAML?



* How do you configure database properties?



* How do you configure server port?



* What are environment profiles?



* How do you activate profiles?



* ###### DevTools



* What is Spring Boot DevTools?



* Why is DevTools used?



* What features does DevTools provide?



* How does DevTools improve development productivity?





* ##### Stage 3 – Web Development



REST API

* What is a REST API?



* What are REST principles?



* What HTTP methods are used in REST?



* What is stateless communication?



* What is idempotency?



Controllers

* What is a controller?



* What is @Controller?



* What is @RestController?



* What is the difference between them?



* How does Spring handle HTTP requests?



Request Mapping



* What is @RequestMapping?



* What are @GetMapping, @PostMapping, @PutMapping, @DeleteMapping?



* What is path mapping?



* How does Spring map URLs to methods?



RequestBody / PathVariable / RequestParam



* What is @RequestBody?



* What is @PathVariable?



* What is @RequestParam?



* What is the difference between them?



* When should each be used?



Example questions often involve:



1. GET /users/{id}
2. POST /users
3. GET /users?page=1
4. Stage 4 – Database Layer
5. Spring Data JPA





* What is Spring Data JPA?



* What problems does it solve?



* What is JpaRepository?



* What CRUD methods does it provide?



* How are custom queries written?



Entity



* What is an Entity?



* What does @Entity do?



* What is @Id?



* What is @GeneratedValue?



* What is the difference between entity and table?



Repository



* What is a repository?



* Why is repository layer needed?



* What is the difference between CrudRepository and JpaRepository?



* How does Spring generate repository implementations?



Hibernate



* What is Hibernate?



* What is ORM?



* What is the role of Hibernate in Spring Boot?



* What is the EntityManager?



* What is lazy loading?



* What is eager loading?



* #### MySQL Integration



* How do you connect Spring Boot to MySQL?



* What properties are required for database connection?



* What does spring.jpa.hibernate.ddl-auto do?



* What is connection pooling?



Stage 5 – Production Topics



DTO Pattern

* What is a DTO?



* Why do we use DTOs?



* What is the difference between DTO and Entity?



* Why should entities not be exposed in APIs?



Validation



* What is validation?



* What is @Valid?



* What is @NotNull?



* What is @NotBlank?



* What is @Size?



* How does Spring handle validation errors?



Exception Handling



* What is global exception handling?



* What is @ControllerAdvice?



* What is @ExceptionHandler?



* How are custom exceptions created?



API Response Wrapper



* Why use a response wrapper?



* What should a standard API response contain?



* What fields are usually included?



* Example structure:



1. status
2. message
3. data
4. timestamp
5. Logging



* Why is logging important?



* What is SLF4J?



* What logging framework does Spring Boot use by default?



* What are logging levels?



1. TRACE
2. DEBUG
3. INFO
4. WARN
5. ERROR

