# Readings

## [Spring App Basics](https://spring.io/guides/gs/serving-web-content/)

### Starting with Spring Initializr

 > Navigate to https://start.spring.io. This service pulls in all the dependencies you need for an application and does most of the setup for you.

> Choose either Gradle or Maven and the language you want to use. This guide assumes that you chose Java.

> Click Dependencies and select Spring Web, Thymeleaf, and Spring Boot DevTools.

> Click Generate.

 > Download the resulting ZIP file, which is an archive of a web application that is configured with your choices.

### Create a webcontroller

```java
package com.example.servingwebcontent;

import org.springframework.stereotype.Controller;
import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RequestParam;

@Controller
public class GreetingController {

	@GetMapping("/greeting")
	public String greeting(@RequestParam(name="name", required=false, defaultValue="World") String name, Model model) {
		model.addAttribute("name", name);
		return "greeting";
	}

}

```

### Spring Boot Devtools

Enables hot swapping.

Switches template engines to disable caching.

Enables LiveReload to automatically refresh the browser.

Other reasonable defaults based on development instead of production.

### Run The Application

The spring initializr creates an application calss for you.

runs the applicaiton

> ./gradlew bootRun.

you can build the JAR file using

> ./gradlew build

and then run the JAR file

> java -jar build/libs/gs-serving-web-content-0.1.0.jar

### Test the Application

Now that the website is created and running head to

> http://localhost:8080/greeting

## Things I want to know more about

Not really learn more but just do all this process on my own.