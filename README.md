
Simple Calculator – Spring Boot & Thymeleaf
A simple web calculator built with Spring Boot and Thymeleaf that performs basic arithmetic operations (Add, Subtract, Multiply, Divide) through a browser UI and REST‑style endpoints.
​
​

Features
Perform basic operations: addition, subtraction, multiplication, division.
​

Validation for division by zero with a clear error message.
​

Simple HTML UI using Thymeleaf templates (home.html, result.html).
​

Layered structure with Controller and Service classes (CalculatorController, CalculatorService).
​

Tech Stack
Java (JDK 21 in this project, configurable).
​

Spring Boot (Spring Web, Thymeleaf).
​

Maven for build and dependency management.
​

Thymeleaf for server‑side HTML rendering.
​

Project Structure
src/main/java/.../CalculatorAppApplication.java – Spring Boot main class.
​

src/main/java/.../controller/CalculatorController.java – handles /api/calculator (GET) and /api/calculate (POST).
​

src/main/java/.../service/CalculatorService.java – business logic for add, sub, mul, div.
​

src/main/resources/templates/home.html – input form for numbers and operation.
​

src/main/resources/templates/result.html – shows result and allows another calculation.
​

Getting Started
Prerequisites
Java 17+ (project currently using Java 21).
​

Maven 3.x installed and on your PATH.
​

Run the application
bash
# clone the repo
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>

# build and run
mvn spring-boot:run
The app starts on http://localhost:9090.
​

Usage
Web UI
Open http://localhost:9090/api/calculator in your browser.
​

Enter Number 1 and Number 2.

Click one of the operation buttons (Add, Subtract, Multiply, Divide).

You are redirected to the result page showing the result and operation.
​

Testing with Postman
URL: POST http://localhost:9090/api/calculate

Body type: x-www-form-urlencoded

Fields:

num1: first number

num2: second number

operation: add | sub | mul | div

The response body contains the rendered HTML of result.html with the calculated value.
​

Future Improvements
Add more operations (square, percentage, power, etc.).
​

Add unit tests for CalculatorService.
​

Add Dockerfile and deployment instructions.
​

