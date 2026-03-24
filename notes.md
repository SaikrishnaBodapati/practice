02-01-2026



bean Level Inheritance - class to class

configuration Level Inheritance









ApplicationContext()

* ClasspathXmlApplicationContext
* FileSystemXmlApplicationContext
* XmlWebApplicationContext

loads the spring bean configuration file , create bean class object and inject the class





@auto wiring
@required annotation
@Qualifier - Qualifier lets you decide which bean to run and we will pass config file reference names as value





@resource - as replacement of the qualifier and autowired we can use the resource rather than using both of them.



Spring Config file



@configuration

@bean

@Postconstructor



Jdbc api

using jdbc api interact with database s/w to perform the manipulations like insert and update ,delete,retrive



JDBC template isa spring helper class that simplifies. JDBC operations such as connection handling, statement creation, and exception handling.

jdbc Template

jdbc Template{DataSource,ds}





**Data Source** is a standard interface in java (JDBC) used to get database connections in a managed , efficient, and scalable way

 usage and advantages



Types of datasource -





DriverManager DataSource



Basic DataSource(Apache DBCP)



Hikari DataSource



JNDI DataSource





JDBC Template ->DML operations



int update(string sql\_stmt,Object... parms)

int update(String sql\_stmt,Object \[] parms)





update(sql\_stmt,"sai","hyd","saikrishna11@gmail.com");





repository - it tells the spring that this class interacts with database



simple jdbc template
bean PropertyROWMapper



Query for xxx() methods







Springboot



traditional spring app need lots of xml configuration









Springboot is an extension of the spring framework  that simplifies the development of standalone , production-ready spring application.



spring boot help you







Spring database JPA

interact with database s/w too perform the manipulations  on DB( update ,delete, retrive)



orm software



Ibaties

EjbEntitiBeans

Hibernate

Hypernate

JPA

SpringDataJPA







20-01-2025



Interface - will perform persistence operations

  types of interfaces

 1)Curd Repository(I) - using this we can perform insert, update, delete, retrive

 2)JPA Repository(I) - crud operations + paging and sorting operations





can you explain the hirerachy in the interface



               Repository(I)

                    |

              |============|

Curd Repository(I)       pagingandsortingRepository(I)

    |                              |

    |                              |

ListCurdRepository       listpagingandsourceRepository     QueryExampleExecutor

                                                                  |

                                                                  |

                                                             JpaRepository





20-01-2026



AllArgsConstructor ( what is constructor)

NoArgsConstructor





App (client)

Entity -customer(Entity class)
Repo   -customerRepository (interface) extend curdrepository
Service - (interface)

ServiceImpl







lombak - help you generate the setter and getter dynamically







configurableApplicationcontext







21-01-2026



 bulit in methods / predefined methods



 

FindBy xxx methods - stands on entity class properties



Eg: to fetch records from the DB using email then we can write

Optional<Entity>FindByEmail(String email)







used to find data using other data(email,number,name) rather than using **FindById**





q1.what is meant by .properties file

q2. what is soft delete

q3. what is CommandLineRunner



q4.Difference between @Component, @Service, and @Repository?



q5.Difference between @Controller and @RestController?



q6.What is @Autowired? How does Spring resolve dependency ambiguity?



q7.Difference between @Qualifier and @Primary?



q8.What is @ConfigurationProperties and why is it better than @Value?



q9.What is @EnableAutoConfiguration?



q10.What is @Bean vs @Component?



q11.What is @PostConstruct and when is it executed?



**simple definition**

soft delete means hiding data instead of permanently deleting it



is\_deleted = true -> record is deleted

is\_deleted = fasle ->record exists



is\_active = true -> record is exist

is\_active = false -> record is deleted





22-01-2026



what is pagination

pagination means dividing a large amount of data into smaller pages instead of loading everything at once.





page object methods



 page.getcontent();

 page.getTotalElements();

 page.getTotalPages();

 page.getNumber();

 page.getsize();

 page.hasNext();

 page.hasPrevious();



\---

spring web mvc( model view controller)





q1.what is mvc design pattern and can you explain the working of the mvc in the project?

q2.what is  Spring Boot dev tool?

q3.what are design patterns in spring web mvc module is developed ?

  mvc design pattern

  front controller Design Pattern

q4.what are built-in controller ?

q5.what are predefined controller?

q6.@controller
q7. @Request Mapping

q8. what is model?

 model  attribute capture the data from view component and carry data to view component

q9.what is @ModelAttribute ?

q10. what is diff b/w model and @modelAttribute

q11.when should we use modelAttribute?

q12. when will you use requestparam?











spring mvc Architecture



 http Request                               http  Response

    ||                                      /\\

    \\/                                      ||

    1                                       10

\-------------------dispatcher servlet----------------

2           3         4      5    6       7      8  9

handler Mapper      Controller    ViewResolver  View





@RequestMapping

Simpler Handler Mapper

bean name handler Mapper

Url based handler mapper

 







@Controller

@AbstractCommandController

@WizardFormController

@MultiActionformController



@ModelAttribute









DispatcherServlet:



Flow (Very Important for Interviews)



Client sends request → /user



DispatcherServlet receives it



Finds matching Controller using HandlerMapping



Calls Controller method



Controller returns:



View name + Model data (or JSON)



ViewResolver finds the actual view



Response sent back to client









q1.pagecontext

q2.jstl

q3.what are implicit objects in jsp ?







**30-01-2025**



##### Distributed Application

============================================================================================================================================================================================

Application interaction with another Application its called as Distributed application



to develop distributed application what are the technologies we can use



EJB - we can only communicate with the application if it was deleveoped or using same language like us

WebServices -



REST- REpresentational State Transfer( created by Roy Fielding) ( transfer the data b/w two parties)



it is a software architectural style created to guide the design of architecture for the web





 client      ->request         server(REST API)    db
<-response



REST Guidelines



CLient Server Architecture

Stateless

cacheable

Layered system

uniform interface

code on demand







resource -

uri - uniform resource identifier





31-01-2026



welcome-message name ( devtools, web)

server.port =8081



WelcomeController



@RestCOntroller/@Controller

@RequestMapping(value="/hellos", method=RequestMethod.get)

@ResponseBody
@GetMapping("/hello") -

@pathVariable-( if we pass a variable with url we call it pathvariable



@RequestParam - Query Parameter is caputured by requestparam





*Spring Frame Work*



* Tight Coupling, loosely coupling
* Dependency injecting \[D.I]
* Inversion of control \[IOC]
* Advantages - POJO , POJI
* non invasive - using poji and pojo is called non invasive
* modular architecture
* Aspect-oriented programming(AOP)
* what is a BeanFactory(I) and what it is used for?

what is meant by .properties file









spring security - 6.X







usernamapasswordAuthenticationFilter

BasicauthenticationFilter























































 

