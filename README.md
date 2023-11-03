# Most-Commonly-Spring-Annotaion
THESE ARE THE MOST COMMONLY USED ANNOTATION IN SPRING BOOT WITH INFORMATION

Spring Boot, being built on the Spring Framework, leverages many annotations to simplify the development of Java applications. Here is an overview of some of the key annotations in Spring Boot and their common uses:

@SpringBootApplication:

	This is the primary annotation that marks a class as a Spring Boot application.
 	It combines @Configuration, @EnableAutoConfiguration, and @ComponentScan annotations.
	It is typically placed on the main application class.

@Controller:

	Annotates a class as a Spring MVC controller,
 	which handles HTTP requests and defines the endpoints for a web application.
	Used in combination with @RequestMapping to specify the URL mappings.

@RestController:

	Similar to @Controller, but it's specifically for building RESTful web services.
	It's often used for creating APIs where the response is automatically serialized to JSON or XML.
	
@Service:

	Indicates that a class is a service component in the application. 
 	Service classes are typically used for business logic and they're injected into controllers or other components.
	
@Repository:

	Marks a class as a repository or data access component. 
 	It's used to interact with databases and perform CRUD operations.
	Spring Boot provides auto-implementation of commonly used data sources.
	
@Component:

	A generic stereotype annotation for any Spring-managed component.
	It's often used for custom beans 
	that don't fall into one of the more specific categories like @Controller or @Service.
	
@Autowired:

	Used to inject dependencies automatically by type. It can be used on fields,
 	setters, and constructors.
	Promotes loose coupling by allowing Spring to manage bean dependencies.
	
@Value:

	Used to inject values from properties files or environment properties into a Spring bean.
	It's commonly used to inject configuration values into application properties.
	
@Configuration:

	Indicates that a class declares Spring beans.
 	It's used in conjunction with @Bean methods to define beans.
	Often used for configuration classes that provide customized configurations.
	
@Bean:

	Used in @Configuration classes to define Spring beans.
 	The return value of a @Bean method becomes a managed bean.
	It's often used to create or configure beans when their creation requires custom logic.
	
@RequestMapping:

	Used to map HTTP requests to specific handler methods in @Controller or @RestController classes.
	It allows you to specify the URL and HTTP method (GET, POST, etc.) for a particular request handler.
	
@PathVariable:

	Used in controller methods to bind a method parameter to a URI template variable.
	It extracts values from the URI path and uses them as method parameters.
	
@RequestParam:

	Binds a method parameter to a query string or form parameter in an HTTP request.
	It allows you to extract data sent in the request parameters.
	
@ModelAttribute:

	Marks a method to add attributes to the model to be used in a view.
 	It's often used in conjunction with @Controller methods.
	
@SessionAttributes:

	Specifies attributes that should be stored in the HTTP session.
 	It's used in conjunction with @Controller methods that use @ModelAttribute.
	
@GetMapping, @PostMapping, etc.:

	Shortcuts for @RequestMapping with specific HTTP methods.
 	For example, @GetMapping is a shortcut for @RequestMapping(method = RequestMethod.GET).
	
@Valid and @Validated:

	Used for method or parameter-level validation.
 	They enable validation on method parameters or return values.
	
@Transactional:

	Marks a method as a transactional method,
	which manages transactions automatically for methods in Spring-managed beans.
	
@ConditionalOnProperty:

	Conditional bean registration based on properties defined in the application's configuration.
	
@Profile:

	Specifies that a component or configuration should be active only when a specific profile is active.
 	Profiles are defined in the application configuration.
	
@EnableAutoConfiguration:

	Enables Spring Boot's auto-configuration mechanism,
 	which automatically configures various beans and settings based on classpath dependencies and properties.
	
These are some of the most commonly used annotations in Spring Boot, 
and they play a significant role in simplifying the development of various types of applications,
whether it's a web application, RESTful API, or a batch processing job.
