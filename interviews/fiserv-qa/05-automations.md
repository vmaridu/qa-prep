# ☕ 05 - Java Automation

## 📌 Overview

- Java is commonly used for automation frameworks, API tests, and Selenium-based suites.
- Maven helps manage dependencies and the build lifecycle.

## 🧱 Java Fundamentals

- Variables, loops, methods, classes, objects
- Collections: List, Set, Map
- OOP concepts: inheritance, polymorphism, encapsulation

Example:

```java
public class Example {
    public static void main(String[] args) {
        List<String> names = Arrays.asList("Alice", "Bob");
        for (String name : names) {
            System.out.println(name);
        }
    }
}
```

## 📦 Maven Basics

- Maven manages dependencies and build lifecycle.
- Common commands:
  - `mvn test`
  - `mvn clean test`
  - `mvn package`

Example `pom.xml` dependency:

```xml
<dependency>
    <groupId>org.testng</groupId>
    <artifactId>testng</artifactId>
    <version>7.8.0</version>
    <scope>test</scope>
</dependency>
```

## 🥒 Cucumber & Gherkin

Example feature file:

```gherkin
Feature: Login
  Scenario: Valid user logs in
    Given user opens the login page
    When user enters valid credentials
    Then dashboard is displayed
```

Example step definition:

```java
@Given("user opens the login page")
public void openLoginPage() {
    System.out.println("Opening login page");
}
```
