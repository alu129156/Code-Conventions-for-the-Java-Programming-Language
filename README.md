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

- [7. References](#7-references)

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
    
## 4.2 Indentation
  
### 4.2.1 Use consistent indentation throughout the code.
    
## 4.3 Comments
  
### 4.3.1 Use comments to explain the purpose of the code.
### 4.3.2 Use Javadoc comments to document classes, methods, and interfaces.
    
## 4.4 Declarations
  
### 4.4.1 Declare variables with the appropriate data type.
### 4.4.2 Use meaningful names for variables.
    
## 4.5 Tasks
  
### 4.5.1 Ensure that all the variables, methods and classes are consistent and do not give contradictions in the different parts of the code.

# 5. Java classes
   
## 5.1 Threads
  
### 5.1.1 Use multithreading for asynchronous and costly tasks like I/O or Database connections.
    
## 5.2 Collection
  
### 5.2.1 Use sets, ArrayLists and Hash Maps to have more optimized and clean code.
    
## 5.3 Sorting Algorithms
  
### 5.3.1 Use the java sorting algorithm library to reduce the code complexity.
    
## 5.4 Exception
  
### 5.4.1 Include exceptions in the code (also create own exceptions), to manage them properly in each class to identify easier the compilation errors.
    
## 5.5 Paths
  
### 5.5.1 Use the path class to have an optimal and automatised access for OS tasks in the code.

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

# 7. References
