# Most-Commonly-Spring-Annotaion
THESE ARE THE MOST COMMONLY USED ANNOTATION IN SPRING BOOT WITH INFORMATION

Spring Boot, being built on the Spring Framework, leverages many annotations to simplify the development of Java applications. Here is an overview of some of the key annotations in Spring Boot and their common uses:

<h3 style="color: aqua;">@SpringBootApplication:</h3>

	This is the primary annotation that marks a class as a Spring Boot application.
 	It combines @Configuration, @EnableAutoConfiguration, and @ComponentScan annotations.
	It is typically placed on the main application class.

<h3 style="color: blue;">@Controller:</h3>

	Annotates a class as a Spring MVC controller,
 	which handles HTTP requests and defines the endpoints for a web application.
	Used in combination with @RequestMapping to specify the URL mappings.

<h3 style="color: brown;">@RestController:</h3>

	Similar to @Controller, but it's specifically for building RESTful web services.
	It's often used for creating APIs where the response is automatically serialized to JSON or XML.
	
<h3 style="color: darkcyan;">@Service:</h3>

	Indicates that a class is a service component in the application. 
 	Service classes are typically used for business logic and they're 
	injected into controllers or other components.
	
<h3 style="color: darkcyan;">@Repository:</h3>

	Marks a class as a repository or data access component. 
 	It's used to interact with databases and perform CRUD operations.
	Spring Boot provides auto-implementation of commonly used data sources.
	
<h3 style="color: lawngreen;">@Component:</h3>

	A generic stereotype annotation for any Spring-managed component.
	It's often used for custom beans 
	that don't fall into one of the more specific categories like @Controller or @Service.
	
<h3 style="color: red;">@Autowired:</h3>

	Used to inject dependencies automatically by type. It can be used on fields,
 	setters, and constructors.
	Promotes loose coupling by allowing Spring to manage bean dependencies.
	
<h3 style="color: brown;">@Value:</h3>

	Used to inject values from properties files or environment properties into a Spring bean.
	It's commonly used to inject configuration values into application properties.
	
<h3 style="color: darkcyan;">@Configuration:</h3>

	Indicates that a class declares Spring beans.
 	It's used in conjunction with @Bean methods to define beans.
	Often used for configuration classes that provide customized configurations.
	
<h3 style="color: darkcyan;">@Bean:</h3>

	Used in @Configuration classes to define Spring beans.
 	The return value of a @Bean method becomes a managed bean.
	It's often used to create or configure beans when their creation requires custom logic.
	
<h3 style="color: brown;">@RequestMapping:</h3>

	Used to map HTTP requests to specific handler methods in @Controller or @RestController classes.
	It allows you to specify the URL and HTTP method (GET, POST, etc.) for a particular request handler.
	
<h3 style="color: brown;">@PathVariable:</h3>

	Used in controller methods to bind a method parameter to a URI template variable.
	It extracts values from the URI path and uses them as method parameters.
	
<h3 style="color: darkcyan;">@RequestParam:</h3>


	Binds a method parameter to a query string or form parameter in an HTTP request.
	It allows you to extract data sent in the request parameters.
	
<h3 style="color: lawngreen;">@ModelAttribute:</h3>

	Marks a method to add attributes to the model to be used in a view.
 	It's often used in conjunction with @Controller methods.
	
<h3 style="color: blue;">@SessionAttributes:</h3>

	Specifies attributes that should be stored in the HTTP session.
 	It's used in conjunction with @Controller methods that use @ModelAttribute.
	
<h3 style="color: blue;">@GetMapping, @PostMapping, etc.:</h3>

	Shortcuts for @RequestMapping with specific HTTP methods.
 	For example, @GetMapping is a shortcut for @RequestMapping(method = RequestMethod.GET).
	
<h3 style="color: lawngreen;">@Valid and @Validated:</h3>

	Used for method or parameter-level validation.
 	They enable validation on method parameters or return values.
	
<h3 style="color: lawngreen;">@Transactional:</h3>

	Marks a method as a transactional method,
	which manages transactions automatically for methods in Spring-managed beans.
	
<h3 style="color: blue;">@ConditionalOnProperty:</h3>

	Conditional bean registration based on properties defined in the application's configuration.
	
<h3 style="color: red;">@Profile:</h3>

	Specifies that a component or configuration should be active only when a specific profile is active.
 	Profiles are defined in the application configuration.
	
<h3 style="color: lawngreen;">@EnableAutoConfiguration:</h3>

	Enables Spring Boot's auto-configuration mechanism,
 	which automatically configures various beans and settings based on classpath dependencies and properties.
	
<b>These are some of the most commonly used annotations in Spring Boot, 
and they play a significant role in simplifying the development of various types of applications,
whether it's a web application, RESTful API, or a batch processing job.<b>
