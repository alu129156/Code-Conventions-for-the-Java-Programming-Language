# Code-Conventions-for-the-Java-Programming-Language
The objective of this project is to create a concise, easy-to-follow Java Code Conventions guide to standardise coding practices, enhance readability, and improve collaboration among Java developers.

- [1. Introduction](#1-introduction)

  - [1.1 Purpose](#11-purpose)
  
    - 1.1.1 The purpose of this guide is to standardize coding practices, enhance readability, and improve collaboration among Java developers.
    
  - [1.2 Scope](#12-scope)
  
    - 1.2.1 This guide applies to all Java code written by the development team.
    
  - [1.3 Definitions](#13-definitions)
  
    - 1.3.1 Naming conventions: A set of rules for choosing names for variables, methods, classes, and packages.
    - 1.3.2 Indentation: The number of spaces used to separate code blocks.
    - 1.3.3 Comments: Text that explains the code and its purpose.
    - 1.3.4 Declarations: Statements that define variables, methods, and classes.
    - 1.3.5 Tasks: Actions or goals that must be performed.

- [2. Coding Practices](#2-coding-practices)

  - [2.1 Naming Conventions](#21-naming-conventions)
  
    * 2.1.1 Use descriptive names for variables, methods, classes, and packages.
    * 2.1.2 Follow the camelCase naming convention for variables and methods.
    * 2.1.3 Follow the PascalCase naming convention for classes and interfaces.
    * 2.1.4 Use all caps for constants.
    
  - [2.2 Indentation](#22-indentation)
  
    - 2.2.1 Use 4 spaces for indentation.
    - 2.2.2 Do not use tabs for indentation.
    
  - [2.3 Comments](#23-comments)
  
    - 2.3.1 Use comments to explain the purpose of the code.
    - 2.3.2 Use Javadoc comments to document classes, methods, and interfaces.
    
  - [2.4 Declarations](#24-declarations)
  
    - 2.4.1 Declare variables at the beginning of the block.
    - 2.4.2 Declare one variable per line.
    
  - [2.5 Tasks](#25-tasks)
  
    - 2.5.1 Data must be encapsulated in the properly classes. All attributes must be private, and it is needed getters and setters.
    - 2.5.2 Correct use of error handling, using Java exceptions.

- [3. Readability](#3-readibility)

  - [3.1 Naming Conventions](#31-naming-conventions)
  
    - 3.1.1 Use meaningful names for variables, methods, classes, and packages.
    - 3.1.2 Avoid using abbreviations or acronyms.
    
  - [3.2 Indentation](#32-indentation)
  
    - 3.2.1 Use consistent indentation throughout the code.
    
  - [3.3 Comments](#33-comments)
  
    - 3.3.1 Use comments to explain the purpose of the code.
    - 3.3.2 Use Javadoc comments to document classes, methods, and interfaces.
    
  - [3.4 Declarations](#34-declarations)

    - 3.4.1 Declare variables with the appropriate data type.
    - 3.4.2 Use meaningful names for variables.
    
  - [3.5 Tasks](#35-tasks)
  
    - 3.5.1 Ensure that the code must be interpreted in a clear and easy way for all the developers.

- [4. Consistency](#4-consistency)

  - [4.1 Naming Conventions](#41-naming-conventions)
  
    - 4.1.1 Use consistent naming conventions throughout the code.
    
  - [4.2 Indentation](#42-indentation)
  
    - 4.2.1 Use consistent indentation throughout the code.
    
  - [4.3 Comments](#43-comments)
  
    - 4.3.1 Use comments to explain the purpose of the code.
    - 4.3.2 Use Javadoc comments to document classes, methods, and interfaces.
    
  - [4.4 Declarations](#44-declarations)
  
    - 4.4.1 Declare variables with the appropriate data type.
    - 4.4.2 Use meaningful names for variables.
    
  - [4.5 Tasks](#45-tasks)
  
    - 4.5.1 Ensure that all the variables, methods and classes are consistent and do not give contradictions in the different parts of the code.

- [5. Java classes](#5-java-classes)
   
  - [5.1 Threads](#51-threads)
  
    - 5.1.1 Use multithreading for asynchronous and costly tasks like I/O or Database connections.
    
  - [5.2 Collection](#52-collection)
  
    - 5.2.1 Use sets, ArrayLists and Hash Maps to have more optimized and clean code.
    
  - [5.3 Sorting Algorithms](#53-sorting-algorithms)
  
    - 5.3.1 Use the java sorting algorithm library to reduce the code complexity.
    
  - [5.4 Exception](#54-exception)
  
    - 5.4.1 Include exceptions in the code (also create own exceptions), to manage them properly in each class to identify easier the compilation errors.
    
  - [5.5 Paths](#55-paths)
  
    - 5.5.1 Use the path class to have an optimal and automatised access for OS tasks in the code.

- [6. Code Checking Process](#6-code-checking-process)

  - [6.1 JUnit test](#61-junit-test)
  
    - 6.1.1 After creating a method, validate it with a JUnit test.
    
  - [6.2 Full class test](#62-full-class-test)
  
    - 6.2.2 After finishing a class, validate it with at least ten different scenarios.

- [7. Tools for Code Conventions Maintenance](#7-tools-for-code-conventions-maintenance)
- [8. References](#8-references)

# 1. Introduction

## 1.1 Purpose
  
### 1.1.1 The purpose of this guide is to standardize coding practices, enhance readability, and improve collaboration among Java developers.
    
## 1.2 Scope
  
### 1.2.1 This guide applies to all Java code written by the development team.
    
## 1.3 Definitions
  
### 1.3.1 Naming conventions: A set of rules for choosing names for variables, methods, classes, and packages.
### 1.3.2 Indentation: The number of spaces used to separate code blocks.
### 1.3.3 Comments: Text that explains the code and its purpose.
### 1.3.4 Declarations: Statements that define variables, methods, and classes.
### 1.3.5 Tasks: Actions or goals that must be performed.

# 2 Coding Practices
## 2.1. Naming Conventions
### 2.1.1 Use descriptive and meaningful names
- **Correct**: `int employeeCount;`
- **Incorrect**: `int ec;`

### 2.1.2 Follow camelCase for variables and methods
- **Correct**: `void calculateSalary() { ... }`
- **Incorrect**: `void CalculateSalary() { ... }`

### 2.1.3 Follow PascalCase for classes and interfaces
- **Correct**: `class EmployeeManager { ... }`
- **Incorrect**: `class employeemanager { ... }`

### 2.1.4 Use all caps for constants
- **Correct**: `static final int MAX_SIZE = 100;`
- **Incorrect**: `static final int MaxSize = 100;`

#### 2.1.5 Avoid abbreviations or acronyms
- **Correct**: `int numberOfPages;`
- **Incorrect**: `int numPgs;`

## 2.2. Indentation

### 2.2.1 Use 4 spaces for indentation
- **Correct**:
  ```java
  if (x == 1) {
      y = 2;
  }
  ```
- **Incorrect** (using 2 spaces):
  ```java
  if (x == 1) {
    y = 2;
  }
  ```

### 2.2.2 Use consistent indentation
- **Correct**:
  ```java
  if (condition) {
      // code
  }
  ```
- **Incorrect** (inconsistent indentation):
  ```java
  if (condition) {
  // code
  }
  ```

### 2.2.3 Do not use tabs for indentation
- **Correct**: (Uses spaces)
- **Incorrect**: (Uses tabs)

## 2.3. Comments

### 2.3.1 Use comments to explain purpose
- **Correct**:
  ```java
  // Calculate the yearly salary
  salary = hoursWorked * hourlyRate;
  ```
- **Incorrect**: (No comment explaining code)

### 2.3.2 Use Javadoc comments for documentation
- **Correct**:
  ```java
  /**
   * Represents an employee in the company.
   */
  public class Employee { ... }
  ```
- **Incorrect**: (No Javadoc comment)

## 2.4. Declarations

### 2.4.1 Declare variables at the beginning
- **Correct**:
  ```java
  void someMethod() {
      int result;
      // code
  }
  ```
- **Incorrect**:
  ```java
  void someMethod() {
      // code
      int result;
  }
  ```

### 2.4.2 Declare one variable per line
- **Correct**:
  ```java
  int count;
  int size;
  ```
- **Incorrect**:
  ```java
  int count, size;
  ```

### 2.4.3 Declare variables with appropriate data type
- **Correct**: `String name = "John";`
- **Incorrect**: `int name = "John";`

## 2.5. Data Encapsulation and Error Handling

### 2.5.1 Encapsulate data in classes
- **Correct**:
  ```java
  public class Employee {
      private String name;

      public String getName() {
          return name;
      }

      public void setName(String name) {
          this.name = name;
      }
  }
  ```
- **Incorrect**:
  ```java
  public class Employee {
      public String name;
  }
  ```

### 2.5.2 Use Java exceptions for error handling
- **Correct**:
  ```java
  try {
      // code that may throw an exception
  } catch (Exception e) {
      // handle exception
  }
  ```
- **Incorrect**:
  ```java
  // code that may throw an exception
  // No exception handling
  ```

## 2.6. Readability and Clarity

### 2.6.1 Ensure clear and interpretable code
- **Correct**: Code with proper naming, indentation, comments, and clear logic.
- **Incorrect**: Code that is hard to read due to lack of comments, poor naming, inconsistent indentation, and convoluted logic.


# 4. Consistency

## 4.1 Naming Conventions
  
### 4.1.1 Use consistent naming conventions throughout the code.
```java
// Example of consistent naming conventions
public class Student {
    private String studentName;
    private int studentAge;
    private double studentGPA;

    public Student(String name, int age, double gpa) {
        this.studentName = name;
        this.studentAge = age;
        this.studentGPA = gpa;
    }

    // Methods follow the same naming convention
    public void updateName(String newName) {
        studentName = newName;
    }

    public void updateAge(int newAge) {
        studentAge = newAge;
    }

    public void updateGPA(double newGPA) {
        studentGPA = newGPA;
    }
}
```
    
## 4.2 Indentation
  
### 4.2.1 Use consistent indentation throughout the code.
```java
// Example of consistent indentation
public class Calculator {
    public int add(int a, int b) {
        return a + b;
    }

    public int subtract(int a, int b) {
        return a - b;
    }

    public int multiply(int a, int b) {
        return a * b;
    }

    public double divide(int a, int b) {
        return (double) a / b;
    }
}
```
    
## 4.3 Comments
  
### 4.3.1 Use comments to explain the purpose of the code.
```java
// This class provides basic arithmetic operations
public class ArithmeticOperations {

    // Adds two integers
    public int add(int a, int b) {
        return a + b;
    }

    // Subtracts the second integer from the first
    public int subtract(int a, int b) {
        return a - b;
    }
}
```
### 4.3.2 Use Javadoc comments to document classes, methods, and interfaces.
```java
/**
 * Represents a basic calculator.
 * Provides methods to perform arithmetic operations.
 */
public class BasicCalculator {

    /**
     * Adds two integers.
     *
     * @param a First operand
     * @param b Second operand
     * @return Sum of a and b
     */
    public int add(int a, int b) {
        return a + b;
    }
}
```
    
## 4.4 Declarations
  
### 4.4.1 Declare variables with the appropriate data type.
```java
public class UserData {
    // Correct data type for each variable
    private String username;
    private int age;
    private double balance;
}
```
### 4.4.2 Use meaningful names for variables.
```java
public class WeatherData {
    // Meaningful variable names
    private double temperatureInCelsius;
    private double windSpeedInKmH;
    private double rainfallInMm;
}
```
    
## 4.5 Tasks
  
### 4.5.1 Ensure that all the variables, methods and classes are consistent and do not give contradictions in the different parts of the code.
```java
public class BankAccount {
    private double accountBalance; // Consistent naming

    public BankAccount(double initialBalance) {
        this.accountBalance = initialBalance; // Consistency in variable usage
    }

    // Method names and functionality are consistent
    public void deposit(double amount) {
        accountBalance += amount;
    }

    public void withdraw(double amount) {
        if (amount <= accountBalance) {
            accountBalance -= amount;
        }
    }
}
```

# 5. Java classes
   
## 5.1 Threads
  
### 5.1.1 Use multithreading for asynchronous and costly tasks like I/O or Database connections.
```java
public class FileProcessor implements Runnable {
    private String filePath;

    public FileProcessor(String filePath) {
        this.filePath = filePath;
    }

    @Override
    public void run() {
        // Simulate a costly I/O operation
        System.out.println("Processing file: " + filePath);
        // File processing logic goes here
    }

    public static void main(String[] args) {
        Thread thread1 = new Thread(new FileProcessor("file1.txt"));
        Thread thread2 = new Thread(new FileProcessor("file2.txt"));

        thread1.start();
        thread2.start();
    }
}
```
    
## 5.2 Collection
  
### 5.2.1 Use sets, ArrayLists and Hash Maps to have more optimized and clean code.
```java
import java.util.*;

public class CollectionExamples {
    public static void main(String[] args) {
        // ArrayList
        List<String> names = new ArrayList<>();
        names.add("Alice");
        names.add("Bob");

        // HashSet
        Set<Integer> uniqueNumbers = new HashSet<>();
        uniqueNumbers.add(1);
        uniqueNumbers.add(2);

        // HashMap
        Map<String, Integer> ageMap = new HashMap<>();
        ageMap.put("Alice", 30);
        ageMap.put("Bob", 35);

        System.out.println("Names: " + names);
        System.out.println("Unique Numbers: " + uniqueNumbers);
        System.out.println("Ages: " + ageMap);
    }
}
```
    
## 5.3 Sorting Algorithms
  
### 5.3.1 Use the java sorting algorithm library to reduce the code complexity.
```java
import java.util.Arrays;

public class SortingExample {
    public static void main(String[] args) {
        int[] numbers = {3, 1, 4, 1, 5, 9};
        Arrays.sort(numbers);
        System.out.println("Sorted Numbers: " + Arrays.toString(numbers));
    }
}
```
    
## 5.4 Exception
  
### 5.4.1 Include exceptions in the code (also create own exceptions), to manage them properly in each class to identify easier the compilation errors.
```java
class UnderAgeException extends Exception {
    public UnderAgeException(String message) {
        super(message);
    }
}

public class ExceptionHandling {
    public static void main(String[] args) {
        try {
            validateAge(15);
        } catch (UnderAgeException e) {
            System.out.println("Caught Exception: " + e.getMessage());
        }
    }

    static void validateAge(int age) throws UnderAgeException {
        if (age < 18) {
            throw new UnderAgeException("Age is less than 18");
        }
        System.out.println("Valid age");
    }
}
```
    
## 5.5 Paths
  
### 5.5.1 Use the path class to have an optimal and automatised access for OS tasks in the code.
```java
import java.nio.file.Path;
import java.nio.file.Paths;

public class PathExample {
    public static void main(String[] args) {
        Path path = Paths.get("C:\\Users\\User\\Documents\\example.txt"); // In Windows
        //Path path = Paths.get("/home/User/documents/example.txt") //On Linux/MacOS
        System.out.println("File Name: " + path.getFileName());
        System.out.println("Root Directory: " + path.getRoot());
        System.out.println("Parent Directory: " + path.getParent());
    }
}
```

# 6. Code Checking Process

## 6.1 JUnit Test

### 6.1.1 Validate methods with JUnit tests

- **Correct**:
  - You have written a method, `int add(int a, int b)`, in a class.
  - You then write a JUnit test for this method:
    ```java
    @Test
    public void testAdd() {
        MyClass myClass = new MyClass();
        assertEquals(5, myClass.add(2, 3));
    }
    ```

- **Incorrect**:
  - You have written a method, `int add(int a, int b)`, in a class.
  - No corresponding JUnit test is written to validate the method.

## 6.2 Full Class Test

### 6.2.2 Validate a class with at least ten different scenarios

- **Correct**:
  - For a class `Calculator`, after fully implementing it, you write multiple JUnit tests covering a range of scenarios:
    - Test adding positive numbers
    - Test adding negative numbers
    - Test adding a positive and a negative number
    - Test multiplying numbers
    - ... (more tests to cover at least ten different scenarios)

  Each test would look like:
  ```java
  @Test
  public void testAddPositiveNumbers() {
      Calculator calc = new Calculator();
      assertEquals(7, calc.add(3, 4));
  }
  // More tests follow...
  ```

- **Incorrect**:
  - For a class `Calculator`, after implementation, only a couple of basic tests are written, not covering the range of functionality:
    - Test adding two numbers
    - Test subtracting two numbers

  There are no tests for edge cases or various other scenarios, falling short of the ten different scenarios guideline.

# 7. Tools for Code Conventions Maintenance
(Add necessary index)

## Extensions for Integrated Development Environments (IDE) like Visual Studio or Eclipse

- **Language Support for Java™ by Red Hat**
  - Provides formatting settings that can be applied in Visual Studio Code.
  - Supports exporting Eclipse formatter files for use in projects.
  - Allows the application of formatter settings from existing profiles such as the Google Style.
  - Offers an editor for editing and previewing formatter settings.

- **Checkstyle for Java**
  - Enables the use of existing Checkstyle configurations or custom files.
  - Provides live linting and quick fixes during Java file editing.

- **SonarLint**
  - An extension that finds and fixes bugs and security issues in Java code.
  - Runs in the background highlighting code issues and providing in-context guidance.
  - Supports over 500 Java rules and includes quick fixes for certain quality issues.

## Web & Desktop Tools

- **Clang-Format**
  - A tool that can create a list of style rules enable programmers to quickly reformat their code and create formatting checks that run on build servers to ensure compliance.
  - It supports several coding standards including LLVM, Google, Chromium, Mozilla, and WebKit.

- **Checkstyle** (also a linting tool so we will extend information later) 
  - A tool to help write Java code adhering to a coding standard.
  - Highly configurable, supporting standards like Sun Code Conventions and Google Java Style.
  - Capable of checking class and method design, code layout, and formatting issues.
  - Available for download from GitHub releases or Maven Central.
  - Also a lightened version is integrable into build processes or development environments via plugins for various IDEs/build tools like Visual Studio, Eclipse, IntelliJ IDEA, Maven, Gradle, and more​​​​​​.


- **Google Java Format**
  - A program that reformats Java source code to comply with Google Java Style.
  - Available for command-line use with options to act on whole files or specific parts.
  - Integrations available for IntelliJ, Android Studio, Eclipse, Gradle, Maven, and more.
  - Does not offer configurability in formatting algorithm, maintaining a unified format.

## Linters [1]

- **Checkstyle**
  - A popular linter that checks Java source code for adherence to a code standard or set of validation rules.
  - Regularly updated with thorough documentation and ample community support.
  - Works natively with Ant and CLI and is available as a plugin for various IDEs and toolsets.
  - Highly configurable XML-based config files to support workflows and production needs.

- **PMD**
  - A static code analyzer emphasizing Java but also supports other languages like JavaScript and Apex.
  - Identifies common programming flaws such as unused variables, empty catch blocks, unnecessary object creation, and more.
  - Features a copy-paste-detector (CPD) for identifying duplicated code across different languages.

- **Error Prone**
  - A tool designed for Java to find potential runtime errors without running the code.
  - Supplements the compiler’s static type checker to catch common Java mistakes as compile-time errors.

- **UCDetector (Unnecessary Code Detector)**
  - Focuses on detecting “dead” code and marking classes for more restricted access modifiers.
  - Useful for optimizing code privacy and preventing unintentional exposure of sensitive field members.

- **Coala**
  - Aims for flexibility and supports linting code in multiple languages including Java.
  - Allows linting using a single config file suitable for multi-language environments.

- **Ckjm**
  - Calculates Chidamber and Kemerer object-oriented metrics by processing the bytecode of compiled Java files​​.

- **Doop**
  - A declarative framework for static analysis of Java/Android programs, focused on pointer analysis algorithms.
  - Provides a wide variety of analyses and scaffolding to run analyses end-to-end​​.

- **SpotBugs**
  - The successor to FindBugs, SpotBugs is a static analysis tool to look for bugs in Java code​​.

- **fb-contrib**
  - A plugin for FindBugs and SpotBugs, offering additional bug detectors​​.

- **JArchitect**
  - Measures, queries, and visualizes Java code to avoid unexpected issues, technical debt, and complexity​​.

‌- **NullAway** 
  - A type-based null-pointer checker with low build-time overhead, acting as an Error Prone plugin​​.

- **Qulice**
  - Combines several pre-configured static analysis tools such as Checkstyle, PMD, and FindBugs​​.


1. *A linter is a software tool used in programming to analyze source code for potential errors, bugs, stylistic errors, and suspicious constructs. The term "linter" originally referred to a program that analyzed C code, but now applies to similar tools for virtually any programming language. Linters perform static analysis, meaning they analyze the code without actually executing it. They help maintain code quality by enforcing coding standards and identifying potential problems like syntax errors, misuse of programming constructs, non-adherence to coding conventions, and potential performance issues. This makes them an essential tool in the software development process for improving and maintaining code quality.*

# 8. References
