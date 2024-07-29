# Spring-in-action-CH1-review
Review of the first chapter of the book Spring in action by Craig Walls

In this chapter we initialize a spring project using spring initializer ((https://start.spring.io/)) 

We include the following depencies: 

- Spring boot stater web
- Thymeleaf
- Spring boot devtools
- Spring boot stater test
- Junit vintage engine


Then we create a Home page controller pointing to an html file using the following code


```
import org.springframework.stereotype.Controller;
import org.springframework.web.bind.annotation.GetMapping;

@Controller 
public class HomeController {

@GetMapping("/") 
 public String home() {
 return "home"; 
 }

}
```