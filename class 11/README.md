**Spring App Basics**

**What role do the @Controller classes play in a Spring MVC application?**

`@Controller` classes are responsible for preparing a model map with data and selecting a view to be rendered

**Explain to a non-technical friend what a GET request is.**

a get request is very similar to the info you tell a waiter to inform him of that you want to order for launch at a restaurant 

where the waiter would take your order to the kitchen and bring back the food you ordered 

**What annotation should be placed on your Spring Boot application class?**

@SpringBootApplication 

**Spring MVC and Thymeleaf**

**What method allows for a variable defined in Java (in your Spring Controller) to be dispalyed in HTML with the help of Thymeleaf?**

@GetMapping("/VariableName")

**Explain the role of a @Controller class in a Spring MVC application.**

 it is transformed into a Thymeleaf context object (part of the Thymeleaf *template execution context*) that makes all the defined variables available to expressions executed in templates.

**What is a model attribute refered to in Thymeleaf?**

it's the attribute that we pass from @Controller class in a Spring MVC application, from  model.addAttribute("name", name);