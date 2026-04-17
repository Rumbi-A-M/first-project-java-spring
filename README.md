First Project – Java Spring Boot (Task 1)
Project Overview

This project was created as part of the Spring Framework coursework (Task 1).
The objective is to build a basic Spring Boot application from scratch, create a controller, and handle HTTP requests.

The application demonstrates:

Creating a Spring Boot project using Spring Initializr
Implementing a simple controller
Handling HTTP requests using @ResponseBody
Returning both plain text and a basic HTML view (MVC pattern)
Technologies Used
Java
Spring Boot
Maven
Spring Web
Thymeleaf
Lombok
Project Setup
1. Clone the repository
git clone https://github.com/Rumbi-A-M/first-project-java-spring.git
cd first-project-java-spring
2. Open in IDE
Open the project in IntelliJ IDEA (recommended)
Reload Maven dependencies
3. Run the application

Run the main class:

FirstProjectJavaSpringApplication.java
Application Usage
Default Endpoint (GET request)

Open in browser:

http://localhost:8080/

Expected result:
A simple text response returned from the controller.

Controller Explanation

Example:

@GetMapping("/")
@ResponseBody
public String home() {
    return "Hello World!";
}

Explanation:

@GetMapping("/") handles HTTP GET requests to the root URL
@ResponseBody ensures the return value is sent directly as the HTTP response
The browser displays the returned string
MVC View Rendering

The project also demonstrates a simple MVC structure where a view is returned.

Endpoint:
http://localhost:8080/greeting

Expected result:

An HTML page rendered using Thymeleaf
The page may include text and an image
Project Structure
src/
 ├── main/
 │   ├── java/
 │   │   └── controller/
 │   │       └── GreetingController.java
 │   ├── resources/
 │   │   ├── templates/
 │   │   │   └── greeting.html
 │   │   └── static/
 │   │       └── image.png
Testing

You can test the application using:

Browser
http://localhost:8080/
http://localhost:8080/greeting
Postman
Send a GET request to:
http://localhost:8080/
Screenshots

Add the following screenshots to meet assignment requirements:

Application running in the IDE
Browser output for localhost:8080
Greeting page with HTML view and image
Learning Outcomes

Through this project, the following concepts were practiced:

Creating and configuring a Spring Boot project
Handling HTTP requests with controllers
Using @ResponseBody
Basic MVC pattern in Spring Boot
Running and testing a Spring application
