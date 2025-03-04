## Navigation
- [Unit 1](#unit-1)
- [Unit 2](#unit-2)
- [Unit 3](#unit-3)
- [Unit 4](#unit-4)
- [Unit 5](#unit-5)


## unit-1
### 1. Introduction to Core Java

Core Java is the fundamental part of Java programming used for general-purpose applications. It includes basic Java concepts like OOP, Memory Management, Exception Handling, Multi-threading, and Collections.

**Key Features of Core Java**:

- **Object-Oriented Programming (OOP)** – Java follows OOP concepts like Encapsulation, Inheritance, Polymorphism, and Abstraction.

- **Platform Independence** – Java code runs on any OS using JVM (Java Virtual Machine).
- **Memory Management** – Java automatically manages memory using Garbage Collection.
- **Multi-threading** – Java allows parallel execution of tasks using threads.
- **Security & Exception Handling** – Java provides built-in exception handling with try-catch and a secure execution environment.

**Example Code in Java:**

```java
class HelloWorld {
    public static void main(String args[]) {
        System.out.println("Welcome to Core Java!");
    }
}
```

**Output**

```java
  Welcome to Core Java!
```

**Uses of Core Java:**  
 ✅ Web Development (Spring Boot, JSP, Servlets)  
 ✅ Android Development (Java for Android Apps)  
 ✅ Enterprise Applications (Banking, E-commerce)

---

### 2. What are Data Types? Explain with 5 Examples.

In Java, data types specify the type of value a variable can store. Java has two categories of data types:

- **Primitive Data Types** (Stores simple values like numbers, characters, boolean)
- **Non-Primitive Data Types** (Stores complex objects like arrays, classes, and interfaces)

1.  Primitive Data Types (Total: 8)

    | Data Type | Size    | Example                        |
    | --------- | ------- | ------------------------------ |
    | byte      | 1 byte  | byte b = 100;                  |
    | short     | 2 bytes | short s = 100;                 |
    | int       | 4 bytes | int num = 100000;              |
    | long      | 8 bytes | long bigNum = 100000000L;      |
    | float     | 4 bytes | float pi = 3.14f;              |
    | double    | 8 bytes | double precise = 3.1415926535; |
    | char      | 2 bytes | char letter = 'A;              |
    | boolean   | 1 bit   | boolean isJavaFun = True;      |

2.  Non-Primitive Data Types  
    These are reference types and include:

    - String: String name = "Java";
    - Arrays: int[] numbers = {1, 2, 3, 4};
    - Classes & Objects: Student s1 = new Student();

    Example:

    ```java
    public class DataTypeExample {
        public static void main(String[] args) {
            int age = 21;             // Integer type
            double price = 99.99;     // Floating-point type
            char grade = 'A';         // Character type
            boolean isPassed = true;  // Boolean type
            String name = "Karan";    // Non-Primitive (String)

            System.out.println("Age: " + age);
            System.out.println("Price: " + price);
            System.out.println("Grade: " + grade);
            System.out.println("Passed: " + isPassed);
            System.out.println("Name: " + name);
        }
    }

    ```

---

### 3. Difference Between C++ and Java

C++ and Java are both **object-oriented programming (OOP) languages**, but they have key differences in syntax, memory management, and features.

#### Key Differences Between C++ and Java

| Feature                     | C++                                           | Java                                    |
| --------------------------- | --------------------------------------------- | --------------------------------------- |
| **Platform Dependency**     | Platform-dependent (compiled for specific OS) | Platform-independent (runs on JVM)      |
| **Memory Management**       | Manual (using `new` and `delete`)             | Automatic (Garbage Collection)          |
| **Multiple Inheritance**    | Supported                                     | Not supported (Uses interfaces)         |
| **Pointers**                | Uses pointers                                 | No direct pointer access (for security) |
| **Compilation & Execution** | Compiled into machine code (`.exe` files)     | Compiled into bytecode (`.class` files) |
| **Exception Handling**      | Optional                                      | Mandatory (`try-catch` blocks)          |
| **Operator Overloading**    | Supported                                     | Not supported                           |
| **GUI Development**         | Uses external libraries                       | Built-in GUI (Swing, JavaFX)            |
| **Use Cases**               | System programming, Game engines              | Web, Mobile, Enterprise applications    |

---

### 4. What is JVM? Explain.

The **Java Virtual Machine (JVM)** is a key component of the Java platform. It is responsible for **executing Java programs** by converting bytecode into machine code.

- JVM stands for **Java Virtual Machine**.
- It allows Java programs to be **platform-independent** (Write Once, Run Anywhere).
- JVM **interprets and compiles** Java bytecode into native machine code.
- It provides **memory management, garbage collection, and security features**.

#### JVM follows **3 main steps**:

1. **Compilation** → Java code is compiled into **bytecode (.class file)** by the Java Compiler (`javac`).
2. **Class Loading** → The JVM **loads bytecode** into memory and verifies it.
3. **Execution** → The JVM **interprets or compiles** bytecode into machine code and executes it.

#### **JVM Architecture**

JVM consists of several components:

1. **Class Loader** – Loads Java classes into memory.
2. **Runtime Memory (Heap & Stack)** – Allocates memory for objects and methods.
3. **Execution Engine** – Converts bytecode into machine code.
4. **Garbage Collector** – Automatically removes unused objects from memory.

#### **Example Code Execution in JVM**

```java
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, JVM!");
    }
}
```

#### **Execution Process:**

javac HelloWorld.java → Compiles Java code into HelloWorld.class (Bytecode).
java HelloWorld → JVM executes the bytecode and prints output.

---

### 5. Explain Single-line and Multi-line Comments in Java.

Comments in Java are non-executable statements that help in code documentation. The compiler ignores comments, and they are only for programmers to understand the code better.

#### Types of Comments in Java:

1.  Single-line Comment (//)
    - Used for short explanations on a single line.
    - Anything written after // on the same line is ignored by the compiler.
    #### Example:
    ```java
    public class CommentsExample {
        public static void main(String[] args) {
            // This is a single-line comment
            System.out.println("Hello, Java!"); // Prints Hello, Java!
        }
    }
    ```
2.  Multi-line Comment (/_ ... _/)

    - Used when you need to write longer descriptions across multiple lines.
      Anything between /_ and _/ is ignored by the compiler.

    #### Example:

    ```java
    public class MultiLineComment {
      public static void main(String[] args) {
      /_ This is a multi-line comment.
      It explains the purpose of the code in detail.  _/
      System.out.println("Multi-line comments example");
      }
    }
    ```

3.  Documentation Comment (/\*_ ... _/)

    - Used for writing detailed documentation about classes and methods.
    - This type of comment is used with the javadoc tool to generate documentation.

    #### Example:

    ```java
    /**
     * This class demonstrates documentation comments.
    * @author  Karan gautam
    * @version 1.0
    */
    public class DocCommentExample {
        /**
         * This method prints a welcome message.
         */
        public static void main(String[] args) {
            System.out.println("Documentation comments example");
        }
    }
    ```

---

### 6. Explain if-else in Java.

The if-else statement in Java is used for decision-making. It allows a program to execute different blocks of code based on a condition.

#### Types of if-else Statements in Java:

1. **Simple if Statement**

   Executes a block of code if the condition is true.
   If the condition is false, it skips the block.

   **Example**:

   ```java
   public class IfExample {
       public static void main(String[] args) {
           int number = 10;
           if (number > 0) { // Condition
               System.out.println("Positive number"); // Executes if true
           }
       }
   }
   ```

2. **if-else Statement**

   If the condition is true, the first block runs.
   If the condition is false, the else block runs.

   #### Example:

   ```java
   public class IfElseExample {
       public static void main(String[] args) {
           int number = -5;
           if (number > 0) {
               System.out.println("Positive number");
           } else {
               System.out.println("Negative number");
           }
       }
   }
   ```

3. if-else-if Ladder

   Used when multiple conditions need to be checked.
   The first true condition is executed, and remaining conditions are skipped.

   #### Example:

   ```java
   public class IfElseIfExample {
       public static void main(String[] args) {
           int marks = 75;

           if (marks >= 90) {
               System.out.println("Grade: A");
           } else if (marks >= 75) {
               System.out.println("Grade: B");
           } else if (marks >= 50) {
               System.out.println("Grade: C");
           } else {
               System.out.println("Fail");
           }
       }
   }
   ```

4. Nested if Statement

   An if condition inside another if.
   Used when multiple conditions must be met before executing a block of code.

   #### Example:

   ```java
   public class NestedIfExample {
       public static void main(String[] args) {
           int age = 20;
           int weight = 55;

           if (age >= 18) {
               if (weight >= 50) {
                   System.out.println("Eligible to donate blood");
               } else {
                   System.out.println("Not enough weight");
               }
           } else {
               System.out.println("Not eligible due to age");
           }
       }
   }
   ```

---

### 7. Explain Conditional Operators.

Conditional operators in Java are used to perform comparisons and logical operations. The primary conditional operators include:

1. **Relational Operators** (Used for comparisons)

   - `>` (Greater than)
   - `<` (Less than)
   - `>=` (Greater than or equal to)
   - `<=` (Less than or equal to)
   - `==` (Equal to)
   - `!=` (Not equal to)

2. **Logical Operators** (Used for combining conditions)

   - `&&` (Logical AND)
   - `||` (Logical OR)
   - `!` (Logical NOT)

     **Example Code:**

   ```java
   public class ConditionalOperatorExample {
       public static void main(String[] args) {
           int a = 10, b = 20;
           System.out.println(a > b); // false
           System.out.println(a < b); // true

           boolean result = (a < b) && (b > 15);
           System.out.println("Result of AND operator: " + result);
       }
   }
   ```

   **Output:**

   ```java
   false
   true
   Result of AND operator: true
   ```

---

## unit-2

### 1. What is the use of the else-if statement? Explain with an example

The else-if statement in Java is used when multiple conditions need to be checked sequentially. It allows us to execute different blocks of code based on different conditions.

**Syntax:**

```java
if (condition1) {
    // Code if condition1 is true
} else if (condition2) {
    // Code if condition2 is true
} else {
    // Code if none of the conditions are true
}

```

**Example**

```java
public class ElseIfExample {
    public static void main(String[] args) {
        int marks = 75;

        if (marks >= 90) {
            System.out.println("Grade: A");
        } else if (marks >= 75) {
            System.out.println("Grade: B");
        } else if (marks >= 50) {
            System.out.println("Grade: C");
        } else {
            System.out.println("Fail");
        }
    }
}
```

**Output:**

```
Grade: B
```

The else-if statement ensures that only one condition executes, improving efficiency and readability.

---

### 2. Difference between while and do-while loop.

| Feature           | while Loop                                                  | do-while Loop                                       |
| ----------------- | ----------------------------------------------------------- | --------------------------------------------------- |
| Execution         | Checks condition first, then executes.                      | Executes first, then checks condition.              |
| Condition Check   | Before entering the loop body.                              | After executing the loop body at least once.        |
| Minimum Execution | May not execute if condition is false initially.            | Executes at least once, even if condition is false. |
| Usage             | Used when the number of iterations is not known in advance. | Used when the loop must run at least once.          |

Example of `while` Loop

```java
public class WhileExample {
    public static void main(String[] args) {
        int i = 1;
        while (i <= 3) {
            System.out.println("Iteration: " + i);
            i++;
        }
    }
}

```

Output:

```
Iteration: 1
Iteration: 2
Iteration: 3

```

Example of do-while Loop

```java
public class DoWhileExample {
    public static void main(String[] args) {
        int i = 1;
        do {
            System.out.println("Iteration: " + i);
            i++;
        } while (i <= 3);
    }
}

```

Output:

```
Iteration: 1
Iteration: 2
Iteration: 3

```

The do-while loop runs at least once, even if the condition is initially false.

---

### 3. What is a class? How to define it?

A class in Java is a blueprint for creating objects. It defines attributes (variables) and behaviors (methods) that objects of that class will have.

Key Features of a Class:

- A class is a template that defines the properties (fields/variables) and methods (functions).
- Objects are created from classes using the new keyword.
- Java follows object-oriented programming (OOP), where everything revolves around classes and objects.

Syntax:

```java
class ClassName {
    // Data members (variables)
    DataType variableName;

    // Methods (functions)
    ReturnType methodName() {
        // Code block
    }
}

```

Example: Defining a Class in Java

```java

// Defining a class
class Car {
    // Data members (attributes)
    String brand;
    int speed;

    // Method (behavior)
    void displayCarInfo() {
        System.out.println("Brand: " + brand);
        System.out.println("Speed: " + speed + " km/h");
    }
}

// Main class
public class ClassExample {
    public static void main(String[] args) {
        Car myCar = new Car(); // Creating an object

        // Assigning values to object properties
        myCar.brand = "Toyota";
        myCar.speed = 120;

        // Calling the method
        myCar.displayCarInfo();
    }
}

```

Output:

```java
Brand: Toyota
Speed: 120 km/h
```

**_Explanation of the Above Code:_**

1. class Car {} → Defines a class named Car.
2. Attributes (String brand, int speed) → Define the properties of a Car object.
3. Method (displayCarInfo()) → Defines behavior (prints car details).
4. Creating an Object (new Car()) → Allocates memory for a Car object.
5. Accessing Attributes (myCar.brand = "Toyota";) → Assigns values to the object.
6. Calling a Method (myCar.displayCarInfo();) → Executes the method.

---

### 4. Write a Short Note on Method Overloading

Method Overloading in Java allows multiple methods to have the same name but with different parameters. It improves code readability and reusability by enabling a class to handle different types of inputs with the same method name.

**Rules for Method Overloading:**

1. Different Number of Parameters → Methods must have a different number of arguments.
2. Different Data Types of Parameters → Methods can have the same number of parameters but different data types.
3. Return Type Doesn’t Matter → Only method name and parameters are considered; return type alone cannot overload a method.

**Example**: Method Overloading in Java

```java
class MathOperations {
    // Method with two integers
    int add(int a, int b) {
        return a + b;
    }

    // Overloaded method with three integers
    int add(int a, int b, int c) {
        return a + b + c;
    }

    // Overloaded method with two double numbers
    double add(double a, double b) {
        return a + b;
    }
}

public class OverloadingExample {
    public static void main(String[] args) {
        MathOperations obj = new MathOperations();

        System.out.println("Sum of 2 integers: " + obj.add(5, 10));
        System.out.println("Sum of 3 integers: " + obj.add(5, 10, 15));
        System.out.println("Sum of 2 double numbers: " + obj.add(5.5, 2.5));
    }
}

```

Output:

```java
Sum of 2 integers: 15
Sum of 3 integers: 30
Sum of 2 double numbers: 8.0


```

**Why Use Method Overloading?**  
 ✔ Increases code efficiency by allowing the same method name for different tasks.  
 ✔ Improves readability by keeping related methods together.  
 ✔ Avoids confusion since method names remain consistent.

---

### 5. Define Constructor? List and Explain Types of Constructors.

A constructor in Java is a special type of method used to initialize objects. It is called automatically when an object is created.

**Key Features of Constructors:**
✔ The constructor name must be the same as the class name.  
✔ It does not have a return type (not even void).  
✔ It is called automatically when an object is created.

**Types of Constructors in Java**

1. Default Constructor (No-Argument Constructor)

   - A constructor that does not take any parameters.
   - Used to initialize default values for object attributes.

   **Example:**

   ```java
   class Student {
       String name;

       // Default constructor
       Student() {
           name = "Unknown";
       }

       void display() {
           System.out.println("Student Name: " + name);
       }
   }

   public class DefaultConstructorExample {
       public static void main(String[] args) {
           Student s1 = new Student(); // Constructor called automatically
           s1.display();
       }
   }

   ```

   **Output:**

   ```java
   Student Name: Unknown

   ```

2. Parameterized Constructor

   - A constructor that accepts arguments to assign values to object attributes.
   - Used when specific values need to be set during object creation.

   Example:

   ```java
   class Car {
       String brand;

       // Parameterized Constructor
       Car(String b) {
           brand = b;
       }

       void display() {
           System.out.println("Car Brand: " + brand);
       }
   }

   public class ParameterizedConstructorExample {
       public static void main(String[] args) {
           Car car1 = new Car("Toyota"); // Passing value to constructor
           car1.display();
       }
   }

   ```

   Output

   ```java
   Car Brand: Toyota
   ```

3. Copy Constructor

   - Used to create a new object by copying values from another object.
     Java does not provide a default copy constructor, so we need to define it manually.

   Example:

   ```java
   class Book {
       String title;

       // Parameterized Constructor
       Book(String t) {
           title = t;
       }

       // Copy Constructor
       Book(Book b) {
           title = b.title;
       }

       void display() {
           System.out.println("Book Title: " + title);
       }
   }

   public class CopyConstructorExample {
       public static void main(String[] args) {
           Book b1 = new Book("Java Programming");
           Book b2 = new Book(b1); // Copying values from b1 to b2

           b1.display();
           b2.display();
       }
   }
   ```

   Output:

   ```java
   Book Title: Java Programming
   Book Title: Java Programming
   ```

---

### 6. What is Garbage Collection in Java?

Garbage Collection (GC) in Java is an automatic memory management process that removes unused objects to free up memory. It helps prevent memory leaks and ensures efficient utilization of system resources.

How Does Garbage Collection Work?

- In Java, memory is allocated dynamically when objects are created using the new keyword.
- When an object is no longer referenced, the Garbage Collector (GC) automatically removes it from memory.
- Java uses a process called Mark and Sweep Algorithm to identify and delete unused objects.

**Example**: Garbage Collection in Action

```java
class GarbageDemo {
    String message;

    GarbageDemo(String msg) {
        message = msg;
    }

    // Finalize method (called before garbage collection)
    protected void finalize() {
        System.out.println("Garbage Collected: " + message);
    }

    public static void main(String[] args) {
        GarbageDemo obj1 = new GarbageDemo("Object 1");
        GarbageDemo obj2 = new GarbageDemo("Object 2");

        // Removing references
        obj1 = null;
        obj2 = null;

        // Requesting Garbage Collection
        System.gc();
    }
}

```

Output\*\*: (May vary depending on JVM)

```java
Garbage Collected: Object 1
Garbage Collected: Object 2
```

How to Invoke Garbage Collection?

1. Automatic by JVM → Happens in the background when needed.
2. Manually Using System.gc(); → Suggests JVM to run GC (but not guaranteed).

---

### 7. What is an Object and How to Define It in Java?

An object is an instance of a class that contains state (attributes/variables) and behavior (methods/functions). Objects allow us to use the properties and methods defined in a class.

**Characteristics of an Object:**
✔ State → Represented by attributes (variables).
✔ Behavior → Defined by methods (functions).
✔ Identity → Each object has a unique reference in memory.

Syntax:

```java
ClassName objectName = new ClassName();

```

- ClassName → The class from which the object is created.
- objectName → The name of the object.
- new → Allocates memory dynamically.
- ClassName() → Calls the constructor of the class.

Example: Creating an Object in Java

```java
class Car {
    // Attributes (State)
    String brand;
    int speed;

    // Method (Behavior)
    void displayCarInfo() {
        System.out.println("Brand: " + brand);
        System.out.println("Speed: " + speed + " km/h");
    }
}

public class ObjectExample {
    public static void main(String[] args) {
        // Creating an object of the Car class
        Car myCar = new Car();

        // Assigning values to object properties
        myCar.brand = "Toyota";
        myCar.speed = 120;

        // Calling a method
        myCar.displayCarInfo();
    }
}

```

Output:

```java
Brand: Toyota
Speed: 120 km/h

```

**_How Objects Work in Memory?_**

- When new Car(); is executed, memory is allocated dynamically.
- myCar is a reference variable that points to the object's memory location.

---

## unit-3

### 1. List and explain types of Inheritance ?

Inheritance is a mechanism in Java where a child class (subclass) acquires properties and behaviors from a parent class (superclass). It allows code reusability and establishes a hierarchical relationship between classes.

Types of Inheritance in Java:

| Type                                     | descriptions                                                                               |
| ---------------------------------------- | ------------------------------------------------------------------------------------------ |
| 1. Single Inheritance                    | One class inherits from another.                                                           |
| 2. Multilevel Inheritance                | A class inherits from another class, which in turn inherits from another class.            |
| 3. Hierarchical Inheritance              | Multiple child classes inherit from a single parent class.                                 |
| 4. Multiple Inheritance (via Interfaces) | A class implements multiple interfaces (Java does not support multiple class inheritance). |
| 5. Hybrid Inheritance                    | A combination of two or more types of inheritance (achieved using interfaces).             |

(i) Single Inheritance
✅ One class inherits from another.

✅ Example:

```java
class Animal{
    vaid eat(){
        System.out.printIn("This animal eats food.");
    }
}

class Dog extends Animal{
 void bark(){
   System.out.printIn("Dog barks!");
 }
}

pubilc class SingleInhertances {
    public static void main(String[] args){
        Dog myDog = new Dog();
        myDog.eat();
        myDog.bark();
    }
}
```

✅ Output:

```java
This animal eats food.
Dog barks!
```

(ii) Multilevel Inheritance
✅ A class inherits from another inherited class.

✅ Example:

```java
class Animal {
    void eat() {
        System.out.println("This animal eats food.");
    }
}

class Mammal extends Animal {
    void sleep() {
        System.out.println("Mammals sleep at night.");
    }
}

class Dog extends Mammal {
    void bark() {
        System.out.println("Dog barks!");
    }
}

public class MultilevelInheritanceDemo {
    public static void main(String[] args) {
        Dog myDog = new Dog();
        myDog.eat();
        myDog.sleep();
        myDog.bark();
    }
}

```

✅ Output:

```java
This animal eats food.
Mammals sleep at night.
Dog barks!

```

(iii) Hierarchical Inheritance
✅ Multiple child classes inherit from a single parent class.

✅ Example:

```java
class Animal {
 void eat() {
 System.out.println("This animal eats food.");
 }
}

class Dog extends Animal {
 void bark() {
 System.out.println("Dog barks!");
 }
}

class Cat extends Animal {
 void meow() {
 System.out.println("Cat meows!");
 }
}

public class HierarchicalInheritanceDemo {
 public static void main(String[] args) {
 Dog myDog = new Dog();
 myDog.eat();
 myDog.bark();

        Cat myCat = new Cat();
        myCat.eat();
        myCat.meow();
    }

}
```

✅ Output:

```java
This animal eats food.
Dog barks!
This animal eats food.
Cat meows!
```

(iv) Multiple Inheritance (Using Interfaces)
✅ Java does not support multiple inheritance with classes, but it can be done using interfaces.

✅ Example:

```java
interface Animal {
 void eat();
}

interface Sound {
 void makeSound();
}

class Dog implements Animal, Sound {
 public void eat() {
 System.out.println("Dog eats food.");
 }

    public void makeSound() {
        System.out.println("Dog barks!");
    }

}

public class MultipleInheritanceDemo {
 public static void main(String[] args) {
 Dog myDog = new Dog();
 myDog.eat();
 myDog.makeSound();
 }
}
```

✅ Output:

```java
Dog eats food.
Dog barks!
```

(v) Hybrid Inheritance (Using Interfaces)
✅ Hybrid Inheritance is a combination of multiple and hierarchical inheritance.

✅ Example:

```java
interface Animal {
 void eat();
}

interface Sound {
 void makeSound();
}

class Mammal implements Animal {
 public void eat() {
 System.out.println("Mammal eats food.");
 }
}

class Dog extends Mammal implements Sound {
 public void makeSound() {
 System.out.println("Dog barks!");
 }
}

public class HybridInheritanceDemo {
 public static void main(String[] args) {
 Dog myDog = new Dog();
 myDog.eat();
 myDog.makeSound();
 }
}
```

✅ Output:

```java
Mammal eats food.
Dog barks!
```

4. Key Points for 5 Marks Answer:   
   ✅ Inheritance allows a child class to acquire properties from a parent class.   
   ✅ It helps in code reusability and reduces redundancy.   
   ✅ Five types of inheritance: Single, Multilevel, Hierarchical, Multiple (via Interfaces), and Hybrid (via Interfaces).   
   ✅ Multiple inheritance is not supported in Java with classes but can be achieved using interfaces.
   ✅ Examples provided for each type.     

---

### 2. Write a short note on Method Overriding with example ?

1. Definition of Method Overriding:
   Method Overriding in Java allows a subclass to redefine a method that is already present in the superclass. The method in the subclass must have:  
   ✔ The same name as in the parent class.  
   ✔ The same parameters as in the parent class.  
   ✔ A different implementation in the child class.

2. Rules for Method Overriding:  
   ✔ The method must have the same name and parameters.  
   ✔ There must be an inheritance relationship (i.e., extends keyword).  
   ✔ The method in the child class cannot have a lower access modifier than the method in the parent class.  
   ✔ static, final, and private methods cannot be overridden.

3. Example of Method Overriding in Java:

   ```java
   // Parent Class
   class Animal {
    void makeSound() {
    System.out.println("Animal makes a sound!");
    }
   }


    // Child Class
    class Dog extends Animal {
        // Overriding the makeSound method
        @Override
        void makeSound() {
        System.out.println("Dog barks!");
        }
    }

    // Main Class
    public class MethodOverridingDemo {
        public static void main(String[] args) {
        Animal myAnimal = new Animal();
        myAnimal.makeSound(); // Calls the method from Animal class

        Dog myDog = new Dog();
        myDog.makeSound(); // Calls the overridden method from Dog class
       }

    }
   ```

   ✅ Output:

   ```
   Animal makes a sound!
   Dog barks!
   ```

4. Why is Method Overriding Useful?  
   ✔ Enables runtime polymorphism (dynamic method dispatch).  
   ✔ Helps in achieving abstraction and flexibility in code.  
   ✔ Allows a subclass to provide a specific implementation.

✅ Example of Runtime Polymorphism:

```java

class Animal {
    void makeSound() {
    System.out.println("Animal makes a sound!");
    }
}

class Dog extends Animal {
    void makeSound() {
    System.out.println("Dog barks!");
    }
}

public class PolymorphismDemo {
public static void main(String[] args) {
    Animal myPet;
    myPet = new Dog();
    myPet.makeSound(); // Calls Dog's overridden method
    }
}
```

✅ Output:

```java
Dog barks!
```

(The method of the subclass is executed instead of the parent class.)

5. Key Points for 5 Marks Answer:   
   ✅ Method overriding allows a child class to redefine a method of the parent class.  
   ✅ The method must have the same name and parameters.  
   ✅ Used for achieving runtime polymorphism.  
   ✅ Cannot override static, final, or private methods.   
   ✅ Examples provided for better understanding.   

---

### 3. State the uses of final keyword ?

1. Introduction to final Keyword:
   The final keyword in Java is a modifier that can be used with variables, methods, and classes to restrict modifications.

2. Uses of final Keyword in Java:
   Use Case Description
3. final Variable Used to declare constants (cannot change the value after initialization).
4. final Method Prevents method overriding in subclasses.
5. final Class Prevents inheritance (no subclass can be created).
   (i) final Variable (Constant in Java)
   ✅ A final variable’s value cannot be changed after initialization.

✅ Example:

```java

class FinalVariableDemo {
 public static void main(String[] args) {
 final int SPEED_LIMIT = 80;
 System.out.println("Speed Limit: " + SPEED_LIMIT);

        // SPEED_LIMIT = 100; // ❌ Error: Cannot change final variable
    }

}
```

✅ Output:

```
Speed Limit: 80
```

✅ Use: Declaring constants such as PI = 3.14 or MAX_USERS = 1000.

(ii) final Method (Prevent Method Overriding)
✅ A final method cannot be overridden by a subclass.

✅ Example:

```java
class Parent {
 final void show() {
 System.out.println("This is a final method.");
 }
}

class Child extends Parent {
 // void show() { ❌ Error: Cannot override final method
 // System.out.println("Trying to override.");
// }
}

public class FinalMethodDemo {
 public static void main(String[] args) {
 Child obj = new Child();
 obj.show();
 }
}
```

✅ Output:

```
This is a final method.
```

✅ Use: When you do not want a subclass to change a method’s implementation.

(iii) final Class (Prevent Inheritance)
✅ A final class cannot be inherited by any subclass.

✅ Example:

```java
    final class Vehicle {
        void display() {
        System.out.println("This is a final class.");
        }
    }

    // class Car extends Vehicle { ❌ Error: Cannot inherit final class
    // }

    public class FinalClassDemo {
        public static void main(String[] args) {
        Vehicle v = new Vehicle();
        v.display();
        }
    }
```

✅ Output:

```
This is a final class.
```

✅ Use: To prevent modification of a class, e.g., String class in Java is final.

3. Key Points for 5 Marks Answer:  
   ✅ The final keyword is used to restrict modifications in Java.     
   ✅ A final variable becomes a constant (value cannot change).    
   ✅ A final method cannot be overridden by subclasses.    
   ✅ A final class cannot be inherited.    
   ✅ Examples provided for better understanding.   

---
### 4. Write a short note on abstract class interface ?

1. Abstract Class in Java
   An abstract class in Java is a class that cannot be instantiated. It is used as a base class to provide common functionality for subclasses.

- Characteristics of an Abstract Class:  
   ✔ Declared using the abstract keyword.  
   ✔ Can have both abstract (without body) and concrete (with body) methods.  
   ✔ Cannot be instantiated directly (objects cannot be created).  
   ✔ Can have constructors and variables (both static and non-static).

Example of an Abstract Class:

```java
abstract class Animal {
abstract void makeSound(); // Abstract method (no body)

    void sleep() { // Concrete method (has body)
        System.out.println("Sleeping...");
    }

}

class Dog extends Animal {
    void makeSound() {
    System.out.println("Dog barks!");
    }
}

public class AbstractClassDemo {
    public static void main(String[] args) {
    Dog myDog = new Dog();
    myDog.makeSound(); // Calls overridden method
    myDog.sleep(); // Calls concrete method from abstract class
    }
}
```

✅ Output:

```java
Dog barks!
Sleeping...
```

2. Interface in Java
   An interface in Java is a fully abstract type that contains only abstract methods (before Java 8). It defines a contract that must be implemented by any class that implements the interface.

- Characteristics of an Interface:  
  ✔ Declared using the interface keyword.  
  ✔ Can only have abstract methods (before Java 8).  
  ✔ Cannot have constructors.  
  ✔ A class implements an interface using the implements keyword.  
  ✔ Supports multiple inheritance.

Example of an Interface:

```java
interface Animal {
    void makeSound(); // Abstract method (no body)
}

class Dog implements Animal {
    public void makeSound() {
    System.out.println("Dog barks!");
    }
}

public class InterfaceDemo {
    public static void main(String[] args) {
    Dog myDog = new Dog();
    myDog.makeSound(); // Calls the implemented method
    }
}
```

✅ Output:

```
Dog barks!
```

3. Difference Between Abstract Class and Interface
   Feature Abstract Class Interface - Methods Can have both abstract and concrete methods Can have only abstract methods (before Java 8) - Variables Can have instance variables Only static and final variables allowed - Inheritance Can extend one class only A class can implement multiple interfaces - Constructors Yes, can have constructors No, cannot have constructors - Usage Used for base class implementation Used for defining behavior (contract)

4. Key Points for 5 Marks Answer:     
   ✅ Abstract Class: Contains both abstract and concrete methods, used for base class functionality.    
   ✅ Interface: Contains only abstract methods (before Java 8), used for defining common behavior.     
   ✅ An abstract class can have constructors and variables, but an interface cannot.     
   ✅ A class can extend only one abstract class but can implement multiple interfaces.    
   ✅ Examples provided for better understanding.   
 
---

### 5. Explain procedure to create user define package in java ?

1. What is a Package in Java?
   A package in Java is a collection of related classes and interfaces. It helps in organizing the code and avoiding name conflicts.

✅ Types of Packages:

Built-in Packages → Provided by Java (e.g., java.util, java.io)
User-Defined Packages → Created by the programmer 2. Steps to Create a User-Defined Package  
Step 1: Create a Package  
✔ Use the package keyword at the top of the Java file.  
✔ Save the file with the package name as the folder name.

Example:

```java
// File: MyPackage/Demo.java
package MyPackage; // Declaring package name

public class Demo {
    public void show() {
    System.out.println("This is a user-defined package!");
    }
}
```

✅ Save this file inside a folder named MyPackage.

Step 2: Compile the Package  
✔ Open the terminal/command prompt and go to the directory where the file is saved.  
✔ Use the following command to compile the package:

```cmd
javac -d . Demo.java
```

✔ This creates a folder MyPackage and stores the compiled Demo.class inside it.

Step 3: Use the Package in Another Class  
✔ Import the package using the import keyword.  
✔ Create an object of the class inside the package.

Example:

```java
// File: Main.java
import MyPackage.Demo; // Importing user-defined package

public class Main {
    public static void main(String[] args) {
    Demo obj = new Demo();
    obj.show(); // Calling the method from the package
    }
}
```

Step 4: Compile and Run the Program  
✔ Compile the program:

```
javac Main.java
```

✔ Run the program:

```
java Main
```

✅ Output:

```
This is a user-defined package!
```

3. Key Points for 5 Marks Answer:   
   ✅ A package is a collection of related classes.    
   ✅ The package keyword is used to create a user-defined package.    
   ✅ Packages help in organizing code and avoiding conflicts.    
   ✅ Use the import keyword to access a package in another class.    
   ✅ Steps: Create → Compile → Import → Use → Run.  

---
### 6. Difference between class and interface ?

A class in Java is a blueprint for creating objects. It defines attributes (variables) and behaviors (methods) that objects will have.

✅ Example of a Class:

```java
class Car {
String brand = "Toyota";

    void showBrand() {
        System.out.println("Car Brand: " + brand);
    }

}

public class ClassExample {
    public static void main(String[] args) {
    Car myCar = new Car(); // Creating an object
    myCar.showBrand();
    }
}
```

✅ Output:

```
Car Brand: Toyota
```

2. What is an Interface?
   An interface is a fully abstract type that defines a contract for a class to implement. It contains only abstract methods (before Java 8).

✅ Example of an Interface:

```java
interface Animal {
    void makeSound(); // Abstract method (no body)
}

class Dog implements Animal {
    public void makeSound() {
    System.out.println("Dog barks!");
    }
}

public class InterfaceExample {
    public static void main(String[] args) {
    Dog myDog = new Dog();
    myDog.makeSound();
    }
}
```

✅ Output:

```
Dog barks!
```

3.  Difference Between Class and Interface  
    Feature Class Interface

- Definition A class is a blueprint for creating objects. An interface defines methods that must be implemented.
- Methods Can have both abstract and concrete - methods. Can have only abstract methods (before Java 8).
- Variables Can have instance variables (both static and non-static).
- Can have only static and final variables.
- Inheritance A class can extend only one class (single inheritance).
- A class can implement multiple interfaces (multiple inheritance).
- Instantiation Objects can be created from a class. Objects cannot be created from an interface.
- Usage Used for object creation and implementation.
- Used for defining behavior (contract).

4. Key Points for 5 Marks Answer:   
   ✅ A class is a blueprint for objects, while an interface defines a contract.    
   ✅ A class can have variables and methods, but an interface can only have abstract methods (before Java 8).    
   ✅ A class supports single inheritance, while an interface supports multiple inheritance.    
   ✅ A class can be instantiated, but an interface cannot.    
   ✅ Examples provided for better understanding.  

---
### 7. Explain how to implement an interface into a class ?

An interface in Java is a collection of abstract methods that a class can implement. It is used to define a contract that a class must follow.

✅ Key Features of Interfaces:  
✔ Declared using the interface keyword.  
✔ Contains only abstract methods (before Java 8).  
✔ A class implements an interface using the implements keyword.  
✔ Supports multiple inheritance.

2. Steps to Implement an Interface in Java
   - Step 1: Define an Interface  
     ✔ An interface is created using the interface keyword.

```java
interface Animal {
void makeSound(); // Abstract method
}
```

Step 2: Implement the Interface in a Class  
✔ A class implements an interface using the implements keyword.  
✔ It must provide implementations for all abstract methods in the interface.

```java

class Dog implements Animal {
public void makeSound() {
System.out.println("Dog barks!");
}
}
```

Step 3: Use the Implemented Class in Main Method  
✔ Create an object of the implementing class and call its methods.

```java
public class InterfaceImplementationDemo {
public static void main(String[] args) {
Dog myDog = new Dog();
myDog.makeSound(); // Calling implemented method
}
}
```

✅ Output:

```
Dog barks!
```

3. Implementing Multiple Interfaces  
   ✔ A class can implement multiple interfaces in Java.

```java
interface Animal {
void makeSound();
}

interface Pet {
void play();
}

class Dog implements Animal, Pet {
public void makeSound() {
System.out.println("Dog barks!");
}

    public void play() {
        System.out.println("Dog is playing!");
    }

}

public class MultipleInterfaceDemo {
    public static void main(String[] args) {
    Dog myDog = new Dog();
    myDog.makeSound();
    myDog.play();
    }
}
```

✅ Output:

```
Dog barks!
Dog is playing!
```

4. Key Points for 5 Marks Answer:    
   ✅ An interface is a collection of abstract methods.    
   ✅ A class implements an interface using the implements keyword.    
   ✅ All abstract methods of an interface must be implemented in the class.    
   ✅ A class can implement multiple interfaces in Java.    
   ✅ Examples provided for better understanding.  
---

## unit-4

### 1. Explain Multithreading ?

Multithreading is a programming technique in which multiple threads execute simultaneously to perform different tasks. It helps in improving performance and resource utilization.

1. Key Features of Multithreading:  
   ✔ Thread: A lightweight process that runs independently.  
   ✔ Parallel Execution: Multiple tasks run at the same time.  
   ✔ Faster Execution: Reduces CPU idle time.  
   ✔ Efficient Resource Utilization: Multiple operations can share resources.

2. Why Use Multithreading?  
   ✔ Better CPU Utilization: Tasks are performed in parallel.  
   ✔ Faster Execution: Reduces waiting time.  
   ✔ Smooth User Experience: UI remains responsive in GUI applications.  
   ✔ Real-world Uses: Used in web servers, gaming, and database management.

3. Creating a Thread in Java  
   There are two ways to create a thread in Java:

   Method 1: Using Thread Class (Extending Thread)

   ```java
   class MyThread extends Thread {
       public void run() {
       System.out.println("Thread is running...");
       }
   }

   public class ThreadExample {
       public static void main(String[] args) {
       MyThread t1 = new MyThread();
       t1.start(); // Starting the thread
       }
   }
   ```

   ✅ Output:

   ```
   Thread is running...
   ```

   ✔ start() method starts a new thread and calls the run() method.

   Method 2: Using Runnable Interface (Implementing Runnable)

   ```java
   class MyRunnable implements Runnable {
       public void run() {
       System.out.println("Thread is running using Runnable interface...");
       }
   }

   public class RunnableExample {
       public static void main(String[] args) {
       MyRunnable myRunnable = new MyRunnable();
       Thread t1 = new Thread(myRunnable);
       t1.start();
       }
   }
   ```

   ✅ Output:

   ```
   Thread is running using Runnable interface...
   ```

   ✔ This method is preferred as it supports multiple inheritance.

   4. Key Points for 5 Marks Answer:   
      ✅ Multithreading allows multiple threads to run concurrently.  
      ✅ It improves performance and resource utilization.    
      ✅ Threads can be created using Thread class or Runnable interface.    
      ✅ start() method is used to begin execution of a thread.    
      ✅ Example programs provided for better understanding.  

---

### 2. Explain thread lifecycle ?

A thread lifecycle represents the different states a thread goes through during its execution. Java provides five main states in the lifecycle of a thread.

1. States of a Thread Lifecycle  
   1️⃣ New (Created) State  
   ✔ When a thread is created using the Thread class but has not started yet.  
   ✔ The thread is in the new state.

   ✅ Example:

   ```java
   Thread t = new Thread(); // Thread created but not started
   ```

   2️⃣ Runnable State  
    ✔ When start() is called, the thread moves to the runnable state.  
    ✔ The thread is ready to run and waiting for CPU time.

   ✅ Example:

   ```java
   t.start(); // Thread is now in the runnable state
   ```

   3️⃣ Running State  
    ✔ When the CPU assigns execution time, the thread enters the running state.  
    ✔ The run() method is executing.

   ✅ Example:

   ```java
   public void run() {
   System.out.println("Thread is running...");
   }
   ```

   4️⃣ Blocked (Waiting) State  
    ✔ If a thread is waiting for a resource (e.g., waiting for I/O), it moves to the blocked state.  
    ✔ It waits until the resource is available.

   ✅ Example:

   ```java
   Thread.sleep(1000); // Thread goes into waiting state for 1 second
   ```

   5️⃣ Terminated (Dead) State  
    ✔ When a thread finishes execution, it moves to the terminated state.  
    ✔ A terminated thread cannot be restarted.

   ✅ Example:

   ```java
   System.out.println("Thread execution completed.");
   ```

2. Thread Lifecycle Diagram
   ```css
   [New] → start() → [Runnable] → CPU Assigned → [Running] → Sleep/Wait → [Blocked] → Execution Done → [Terminated]
   ```
3. Example Program Demonstrating Thread Lifecycle

   ```java
   class MyThread extends Thread {
   public void run() {
   System.out.println("Thread is running...");
   }
   }

   public class ThreadLifecycleDemo {
   public static void main(String[] args) {
   MyThread t1 = new MyThread(); // New State
   t1.start(); // Runnable State

           try {
               Thread.sleep(1000);  // Blocked (Waiting) State
           } catch (InterruptedException e) {
               System.out.println(e);
           }

           System.out.println("Thread execution completed."); // Terminated State
       }

   }
   ```

   ✅ Output:

   ```mathematica
   Thread is running...
   Thread execution completed.
   ```

4. Key Points for 5 Marks Answer:    
   ✅ A thread has five main states: New, Runnable, Running, Blocked, and Terminated.    
   ✅ start() moves a thread from New to Runnable state.    
   ✅ A thread runs when CPU assigns time; otherwise, it stays in Runnable state.   
   ✅ sleep() or wait() moves a thread to Blocked state.    
   ✅ A thread enters Terminated state when execution is completed.   
   ✅ Example program demonstrates thread lifecycle. 

---

### 3. Explain two way of creating thread ?

A thread is a lightweight process that runs independently to perform a specific task. Java provides two ways to create a thread:

1️⃣ Extending the Thread class  
2️⃣ Implementing the Runnable interface

2. Method 1: Extending the Thread Class  
   ✔ A new class is created by extending the Thread class.  
   ✔ The run() method is overridden to define the task of the thread.  
   ✔ The start() method is called to begin execution.

✅ Example:

```java
class MyThread extends Thread {
    public void run() {
    System.out.println("Thread is running...");
    }
}

public class ThreadExample {
    public static void main(String[] args) {
    MyThread t1 = new MyThread();
    t1.start(); // Starting the thread
    }
}
```

✅ Output:

```arduino
Thread is running...
```

Advantages of Extending Thread Class  
 ✔ Simple and easy to implement.  
 ✔ Allows direct access to Thread methods.

Disadvantages  
❌ Cannot extend another class (Java does not support multiple inheritance).

3. Method 2: Implementing the Runnable Interface
   ✔ A class implements the Runnable interface.
   ✔ The run() method is overridden to define the thread’s task.
   ✔ A Thread object is created using an instance of the class.

✅ Example:

```java
class MyRunnable implements Runnable {
    public void run() {
    System.out.println("Thread is running using Runnable interface...");
    }
}

public class RunnableExample {
    public static void main(String[] args) {
    MyRunnable myRunnable = new MyRunnable();
    Thread t1 = new Thread(myRunnable);
    t1.start();
    }
}
```

✅ Output:

```
Thread is running using Runnable interface...
```

Advantages of Implementing Runnable Interface  
✔ Supports multiple inheritance as the class can extend another class.  
✔ More flexible and preferred in real-world applications.

Disadvantages  
❌ Requires creating a Thread object separately.

4. Key Differences Between Thread and Runnable
   - Feature Thread Class Runnable Interface
   - Inheritance Cannot extend another class Can extend another class
   - Flexibility Less flexible More flexible
   - Reusability Less reusable More reusable
   - Preferred For Small applications Large applications
5. Key Points for 5 Marks Answer:   
   ✅ A thread can be created using the Thread class or Runnable interface.    
   ✅ Thread class is simple but does not support multiple inheritance.    
   ✅ Runnable interface is flexible and preferred in real-world applications.    
   ✅ Example programs provided for both methods.    
   ✅ Comparison table explains the key differences.

---

### 4. Write a short note on thread synchronization ?

✔ Thread synchronization is a mechanism that ensures that multiple threads do not access shared resources (like variables or objects) at the same time.  
✔ It helps in preventing data inconsistency and ensures thread safety.  
✔ Java provides the synchronized keyword to control access to critical sections of code.

2. Why is Synchronization Needed?
   ✔ When multiple threads access and modify shared data, inconsistent results may occur.  
   ✔ Example: Imagine a bank account where two threads try to withdraw money at the same time. If synchronization is not used, both threads may withdraw money, leading to incorrect balance calculations.

✅ Problem Example (Without Synchronization):

```java
class BankAccount {
int balance = 5000;

    void withdraw(int amount) {
        if (balance >= amount) {
            System.out.println(Thread.currentThread().getName() + " is withdrawing...");
            balance -= amount;
            System.out.println("Remaining balance: " + balance);
        } else {
            System.out.println("Insufficient balance!");
        }
    }

}

public class WithoutSync {
public static void main(String[] args) {
BankAccount account = new BankAccount();

        Thread t1 = new Thread(() -> account.withdraw(3000), "User1");
        Thread t2 = new Thread(() -> account.withdraw(3000), "User2");

        t1.start();
        t2.start();
    }

}
```

❌ Problem: Both threads might withdraw without waiting for the other, leading to incorrect balance calculations.

3. How to Implement Synchronization in Java?
   ✔ Use the synchronized keyword to lock a method or block so that only one thread can access it at a time.

✅ Solution (With Synchronization):

```java
class BankAccount {
int balance = 5000;

    synchronized void withdraw(int amount) { // Synchronized method
        if (balance >= amount) {
            System.out.println(Thread.currentThread().getName() + " is withdrawing...");
            balance -= amount;
            System.out.println("Remaining balance: " + balance);
        } else {
            System.out.println("Insufficient balance!");
        }
    }

}

public class WithSync {
public static void main(String[] args) {
BankAccount account = new BankAccount();

        Thread t1 = new Thread(() -> account.withdraw(3000), "User1");
        Thread t2 = new Thread(() -> account.withdraw(3000), "User2");

        t1.start();
        t2.start();
    }

}
```

✅ Output (Thread Safe Execution):

```cmd
User1 is withdrawing...
Remaining balance: 2000
User2 is withdrawing...
Insufficient balance!
```

✔ Now, only one thread withdraws first, and the other waits until it finishes.

4. Types of Synchronization in Java  
   1️⃣ Method Synchronization: Using synchronized keyword in a method.  
   2️⃣ Block Synchronization: Using synchronized block inside a method.

✅ Example of Block Synchronization:

```java
class BankAccount {
int balance = 5000;

    void withdraw(int amount) {
        synchronized (this) { // Synchronized block
            if (balance >= amount) {
                System.out.println(Thread.currentThread().getName() + " is withdrawing...");
                balance -= amount;
                System.out.println("Remaining balance: " + balance);
            } else {
                System.out.println("Insufficient balance!");
            }
        }
    }

}
```

✔ Block synchronization locks only a specific part of the method, making it more efficient.

5. Key Points for 5 Marks Answer:  
   ✅ Thread synchronization prevents multiple threads from accessing shared resources simultaneously.  
   ✅ It avoids data inconsistency and ensures thread safety.  
   ✅ Synchronization can be achieved using the synchronized keyword (method or block).  
   ✅ Example of a bank account problem shows the need for synchronization.  
   ✅ Block synchronization improves efficiency over method synchronization.

---

### 5. Explain the need of exception handling in java ?

✔ Exception handling is a mechanism in Java used to handle runtime errors and prevent the program from crashing.  
✔ An exception is an unexpected event that disrupts the normal flow of the program.  
✔ Java provides a structured way to detect and handle exceptions using the try, catch, finally, throw, and throws keywords.

2. Why is Exception Handling Needed?
   1️⃣ To Prevent Program Crashes  
   ✔ If exceptions are not handled, the program will terminate unexpectedly.  
   ✔ Example: Dividing a number by zero causes an ArithmeticException.

✅ Example (Without Exception Handling - Program Crashes)

```java
public class ExceptionDemo {
public static void main(String[] args) {
int a = 10, b = 0;
int c = a / b; // Division by zero error
System.out.println("Result: " + c); // This line will not execute
}
}
```

❌ Output:

```pgsql
Exception in thread "main" java.lang.ArithmeticException: / by zero
```

✔ The program stops execution due to an exception.

2️⃣ To Handle Runtime Errors Gracefully  
✔ Exception handling ensures that the program continues execution even after an error occurs.

✅ Example (With Exception Handling - Program Runs Smoothly)

```java
public class ExceptionDemo {
    public static void main(String[] args) {
    int a = 10, b = 0;
        try {
            int c = a / b; // Code that may cause an exception
            System.out.println("Result: " + c);
        } catch (ArithmeticException e) {
         System.out.println("Cannot divide by zero!"); // Handling the error
        }
     System.out.println("Program continues execution...");
    }
}
```

✅ Output:

```csharp
Cannot divide by zero!
Program continues execution...
```

✔ Instead of crashing, the program handles the error and continues running.

3️⃣ To Ensure Proper Resource Management  
✔ If an exception occurs while accessing a file or database, resources may not close properly, causing memory leaks.  
✔ The finally block ensures resources are closed even if an exception occurs.

✅ Example:

```java
import java.io.\*;

public class FileHandlingExample {
    public static void main(String[] args) {
    FileReader file = null;
        try {
            file = new FileReader("test.txt");
            BufferedReader br = new BufferedReader(file);
            System.out.println(br.readLine());
        } catch (IOException e) {
            System.out.println("File not found!");
        } finally {
            try {
            if (file != null) {
                file.close(); // Ensuring resource closure
            }
            } catch (IOException e) {
                System.out.println("Error closing file!");
            }
        }
    }
}
```

✔ The finally block ensures the file is closed even if an exception occurs.

4️⃣ To Maintain Code Readability and Debugging  
✔ Without exception handling, programmers would have to manually check every operation for errors, making code complex and unreadable.  
✔ Using try-catch blocks keeps the code clean and easy to debug.

3. Key Exception Handling Keywords in Java
   - Keyword Purpose
   - try Defines the block of code where an exception may occur.
   - catch Catches and handles the exception.
   - finally A block that always executes, used to close resources.
   - throw Used to manually throw an exception.
   - throws Declares exceptions that a method might throw.
4. Key Points for 5 Marks Answer:
   ✅ Exception handling ensures that the program does not crash due to runtime errors.
   ✅ It allows smooth execution even if an error occurs.
   ✅ It helps manage resources properly using the finally block.
   ✅ It improves code readability and debugging.
   ✅ Example programs demonstrate the importance of exception handling.

---

### 6. Difference between throw and throws ?

In Java, throw and throws are used for exception handling, but they serve different purposes:

✔ throw → Used inside a method to explicitly throw an exception.  
✔ throws → Used in method declaration to indicate that a method may throw exceptions.

2. Difference Between throw and throws
   | Feature | throw | throws |
   |----------------|-------------------------------------------|---------------------------------------------|
   | **Purpose** | Used to throw an exception manually inside a method or block. | Used in method signature to declare that a method may throw exceptions. |
   | **Usage** | Inside a method or block. | In method declaration. |
   | **Syntax** | `throw new ExceptionType("Message");` | `public void method() throws ExceptionType { }` |
   | **Exception Type** | Can throw a single exception at a time. | Can declare multiple exceptions separated by commas. |
   | **Execution Control** | Immediately stops execution and transfers control to the nearest catch block. | Does not stop execution, just informs that a method may throw an exception. |

3. Example of throw (Throwing an Exception Manually)
   ✅ Code Example:

```java
public class ThrowExample {
static void checkAge(int age) {
if (age < 18) {
throw new ArithmeticException("Not eligible to vote!"); // Throwing exception manually
} else {
System.out.println("Eligible to vote.");
}
}

    public static void main(String[] args) {
        checkAge(16); // This will throw an exception
    }

}
```

✅ Output:

```pgsql

Exception in thread "main" java.lang.ArithmeticException: Not eligible to vote!
```

✔ The throw statement stops execution and throws an ArithmeticException.

4. Example of throws (Declaring an Exception in a Method)
   ✅ Code Example:

```java
import java.io.\*;

public class ThrowsExample {
    static void readFile() throws IOException { // Declaring exception
    FileReader file = new FileReader("test.txt");
    BufferedReader br = new BufferedReader(file);
    System.out.println(br.readLine());
    file.close();
    }

    public static void main(String[] args) {
        try {
            readFile(); // Calling method that may throw an exception
        } catch (IOException e) {
            System.out.println("File not found!");
        }
    }

}
```

✅ Output:

```arduino
File not found!
```

✔ The method readFile() declares an exception using throws, but handling is done in main() using try-catch.

5. Key Points for 5 Marks Answer  
   ✅ throw is used inside a method to explicitly throw an exception.  
   ✅ throws is used in method declaration to indicate exceptions that may occur.  
   ✅ throw stops execution immediately; throws does not.  
   ✅ Example of throw: Voting eligibility check.  
   ✅ Example of throws: File reading operation.

---

### 7. Write a short note on custom exception ?

✔ Exception handling is a mechanism in Java used to handle runtime errors and prevent the program from crashing.  
✔ An exception is an unexpected event that disrupts the normal flow of the program.  
✔ Java provides a structured way to detect and handle exceptions using the try, catch, finally, throw, and throws keywords.

2. Why is Exception Handling Needed?  
   1️⃣ To Prevent Program Crashes  
   ✔ If exceptions are not handled, the program will terminate unexpectedly.  
   ✔ Example: Dividing a number by zero causes an ArithmeticException.

✅ Example (Without Exception Handling - Program Crashes)

```java
public class ExceptionDemo {
    public static void main(String[] args) {
    int a = 10, b = 0;
    int c = a / b; // Division by zero error
    System.out.println("Result: " + c); // This line will not execute
    }
}
```

❌ Output:

```pgsql
Exception in thread "main" java.lang.ArithmeticException: / by zero
```

✔ The program stops execution due to an exception.

2️⃣ To Handle Runtime Errors Gracefully  
✔ Exception handling ensures that the program continues execution even after an error occurs.

✅ Example (With Exception Handling - Program Runs Smoothly)

```java
public class ExceptionDemo {
    public static void main(String[] args) {
    int a = 10, b = 0;
        try {
        int c = a / b; // Code that may cause an exception
         System.out.println("Result: " + c);
        } catch (ArithmeticException e) {
         System.out.println("Cannot divide by zero!"); // Handling the error
        }
    System.out.println("Program continues execution...");
    }
}
```

✅ Output:

```csharp
Cannot divide by zero!
Program continues execution...
```

✔ Instead of crashing, the program handles the error and continues running.

3️⃣ To Ensure Proper Resource Management  
✔ If an exception occurs while accessing a file or database, resources may not close properly, causing memory leaks.  
✔ The finally block ensures resources are closed even if an exception occurs.

✅ Example:

```java
import java.io.\*;

public class FileHandlingExample {
    public static void main(String[] args) {
    FileReader file = null;
    try {
        file = new FileReader("test.txt");
        BufferedReader br = new BufferedReader(file);
        System.out.println(br.readLine());
    } catch (IOException e) {
        System.out.println("File not found!");
    } finally {
        try {
            if (file != null) {
                file.close(); // Ensuring resource closure
            }
            } catch (IOException e) {
                System.out.println("Error closing file!");
            }
        }
    }
}
```

✔ The finally block ensures the file is closed even if an exception occurs.

4️⃣ To Maintain Code Readability and Debugging  
✔ Without exception handling, programmers would have to manually check every operation for errors, making code complex and unreadable.  
✔ Using try-catch blocks keeps the code clean and easy to debug.

3. Key Exception Handling Keywords in Java
   - Keyword Purpose
   - try Defines the block of code where an exception may occur.
   - catch Catches and handles the exception.
   - finally A block that always executes, used to close resources.
   - throw Used to manually throw an exception.
   - throws Declares exceptions that a method might throw.
4. Key Points for 5 Marks Answer:  
   ✅ Exception handling ensures that the program does not crash due to runtime errors.  
   ✅ It allows smooth execution even if an error occurs.  
   ✅ It helps manage resources properly using the finally block.  
   ✅ It improves code readability and debugging.  
   ✅ Example programs demonstrate the importance of exception handling.
---

## unit-5

### 1. What is the use of panel ?

✔ A Panel in Java is a container used to group and organize components (like buttons, labels, text fields) inside a GUI window.
✔ It is a part of AWT (Abstract Window Toolkit) and is defined by the Panel class in the java.awt package.
✔ Panels do not have their own window; they are placed inside another container like a Frame or Applet.

1. Uses of a Panel in Java  
   ✅ 1️⃣ To Organize Components  
   ✔ Panels help in arranging components in a structured manner.  
   ✔ Example: In a registration form, we can use separate panels for personal details, address, and contact details.

   ✅ 2️⃣ To Apply Layouts  
    ✔ We can apply different layout managers (like FlowLayout, GridLayout, BorderLayout) to arrange components inside a panel.

   ✅ 3️⃣ To Group Components  
    ✔ If we have related buttons or labels, we can group them inside a panel instead of adding them directly to the main window.

   ✅ 4️⃣ To Improve Code Maintainability  
    ✔ Using panels makes the code modular and easy to manage because different sections of the UI can be handled separately.

2. Example Program Using a Panel  
   ✅ Program to Create a Panel with Buttons

   ```java
   import java.awt._;
   import javax.swing._;

   public class PanelExample {
   public static void main(String[] args) {
   JFrame frame = new JFrame("Panel Example"); // Creating Frame
   frame.setSize(400, 200);

           JPanel panel = new JPanel(); // Creating Panel
           panel.setBackground(Color.LIGHT_GRAY); // Setting Panel Background

           // Adding buttons to panel
           panel.add(new JButton("Button 1"));
           panel.add(new JButton("Button 2"));
           panel.add(new JButton("Button 3"));

           frame.add(panel); // Adding Panel to Frame
           frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
           frame.setVisible(true);
       }

   }
   ```

✅ Output:

✔ A GUI window with three buttons placed inside a light gray panel.

4. Key Methods of Panel Class

- Method Description
- add(Component c) Adds a component to the panel.
- setLayout(LayoutManager l) Sets the layout for the panel.
- setBackground(Color c) Sets the background color of the panel.

5. Key Points for 5 Marks Answer  
   ✅ A panel is a container used to organize and group components in Java GUI.  
   ✅ It is part of the AWT package and is placed inside frames or applets.  
   ✅ Panels help in applying layouts and improve UI structure.  
   ✅ Example program with buttons inside a panel.  
   ✅ Key methods like add(), setLayout(), and setBackground().
---

### 2. Difference between Java applets and Java application?

✔ Java programs can be categorized into Applets and Applications based on their execution environment.  
✔ Java Applet is a small program that runs inside a web browser or applet viewer.  
✔ Java Application is a standalone program that runs directly on the JVM (Java Virtual Machine).

2. Difference Between Java Applet and Java Application
   | Feature | Java Applet | Java Application |
   |----------------------|------------------------------------------------|----------------------------------------------|
   | **Execution** | Runs inside a web browser or an applet viewer. | Runs independently on the JVM. |
   | **Main Method** | Does not use the `main()` method. | Uses the `main()` method as the entry point. |
   | **Security Restrictions** | Runs in a sandbox environment with restricted access to system resources. | Has full access to system resources like files, network, and databases. |
   | **User Interface** | Uses AWT (Abstract Window Toolkit) for GUI. | Can use Swing, JavaFX, or AWT for GUI. |
   | **Performance** | Slower due to browser dependency. | Faster and more efficient. |
   | **Internet Dependency** | Requires an HTML page and a browser. | Does not require a browser. |
   | **Examples** | Online games, calculators, animations. | Desktop applications like Notepad, Word Processors, Games. |

3. Example of a Java Applet  
   ✅ Simple Applet to Display "Hello, Applet!"

```java
import java.applet.Applet;
import java.awt.Graphics;

public class MyApplet extends Applet {
    public void paint(Graphics g) {
    g.drawString("Hello, Applet!", 50, 50);
    }
}
```

✔ How to Run: Save the file as MyApplet.java and compile it. Then, create an HTML file:

```html
<applet code="MyApplet.class" width="200" height="100"></applet>
```

✔ Open the HTML file in a browser that supports Java applets (or use appletviewer).

4. Example of a Java Application
   ✅ Simple Java Application to Print "Hello, World!"

```java
public class MyApp {
    public static void main(String[] args) {
    System.out.println("Hello, World!");
    }
}
```

✔ How to Run: Compile and run using:

```nginx
javac MyApp.java
java MyApp
```

5. Key Points for 5 Marks Answer  
   ✅ Java Applet runs in a web browser, while Java Application runs independently.  
   ✅ Applets do not use main(), but Applications do.  
   ✅ Applets have security restrictions; Applications have full system access.
   ✅ Example Applet: Displays "Hello, Applet!"  
   ✅ Example Application: Prints "Hello, World!" on console.

---
### 3. Write a short note on border layout ?

✔ BorderLayout is one of the layout managers in Java's AWT (Abstract Window Toolkit).
✔ It divides the container into five regions:

- NORTH (Top)
- SOUTH (Bottom)
- EAST (Right)
- WEST (Left)
- CENTER (Middle)

✔ Components are placed in these regions, and the layout automatically arranges them.

2.  Syntax of BorderLayout

    ```java
    Container.setLayout(new BorderLayout());
    ```

    ✔ This method sets BorderLayout as the layout manager for the container.

3.  Example Program Using BorderLayout  
     ✅ Java Program to Demonstrate BorderLayout

        ```java
        import java.awt._;
        import javax.swing._;

        public class BorderLayoutExample {
        public static void main(String[] args) {
        JFrame frame = new JFrame("BorderLayout Example");
        frame.setSize(400, 300);

                frame.setLayout(new BorderLayout()); // Setting BorderLayout

                frame.add(new JButton("NORTH"), BorderLayout.NORTH);
                frame.add(new JButton("SOUTH"), BorderLayout.SOUTH);
                frame.add(new JButton("EAST"), BorderLayout.EAST);
                frame.add(new JButton("WEST"), BorderLayout.WEST);
                frame.add(new JButton("CENTER"), BorderLayout.CENTER);

                frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
                frame.setVisible(true);
            }

        }
        ```

    ✅ Output:
    ✔ A window with five buttons arranged in BorderLayout.

4.  Key Methods of BorderLayout
    - Method Description
    - add(Component, BorderLayout.Position) Adds a component to a specific region.

- setHgap(int gap) Sets horizontal space between components.
- setVgap(int gap) Sets vertical space between components.

5. Advantages of BorderLayout  
   ✔ Automatically resizes components when the window is resized.  
   ✔ Simple to use and easy to arrange components.  
   ✔ No need to specify exact positions for components.

6. Key Points for 5 Marks Answer  
   ✅ BorderLayout divides a container into five regions: NORTH, SOUTH, EAST, WEST, CENTER.  
   ✅ Components are automatically arranged in these regions.  
   ✅ Example program with buttons placed in each region.  
   ✅ Key methods: add(), setHgap(), setVgap().  
   ✅ BorderLayout is useful for creating structured UI layouts.

---

### 4. List any 5 event classes ?

✔ In Java, an event is an action that occurs when a user interacts with a GUI component (e.g., clicking a button, pressing a key).  
✔ Java provides a package java.awt.event that contains various event classes.  
✔ These event classes are used to handle different types of events in GUI applications.

2. Five Important Event Classes in Java

- Event Class Description
- ActionEvent Generated when a user clicks a button or selects a menu item.
- MouseEvent Occurs when a user clicks, presses, releases, or moves the mouse.
- KeyEvent Generated when a key is pressed or released on the keyboard.
- WindowEvent Occurs when a window is opened, closed, minimized, or maximized.
- ItemEvent Triggered when a user selects or deselects an item in a checkbox, list, or menu.

3. Example: Handling ActionEvent  
   ✅ Java Program for Button Click Event

   ```java
   import java.awt._;
   import java.awt.event._;
   import javax.swing.\*;

   public class EventExample extends JFrame implements ActionListener {
   JButton button;

       public EventExample() {
           button = new JButton("Click Me");
           button.addActionListener(this); // Register event listener
           add(button);
           setSize(300, 200);
           setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
           setVisible(true);
       }

       public void actionPerformed(ActionEvent e) {
           System.out.println("Button Clicked!");
       }

       public static void main(String[] args) {
           new EventExample();
       }

   }
   ```

   ✅ Output:  
    ✔ When the user clicks the "Click Me" button, the message "Button Clicked!" is printed on the console.

4. Key Points for 5 Marks Answer  
   ✅ Event classes are used to handle user interactions in GUI applications.  
   ✅ Five important event classes: ActionEvent, MouseEvent, KeyEvent, WindowEvent, and ItemEvent.  
   ✅ Each class is used for specific user actions like clicking a button, pressing a key, or closing a window.  
   ✅ Example program demonstrating ActionEvent.  
   ✅ Event handling is done using listeners like ActionListener.

---

### 5. Explain card layout with program ?

✔ CardLayout is a layout manager in Java AWT that allows switching between multiple panels (like cards).  
✔ It is useful when you want to display one panel at a time, such as in a tabbed interface or a wizard-style application.  
✔ It stores multiple components and lets you navigate between them.

2. Syntax of CardLayout

   ```java
   Container.setLayout(new CardLayout());
   ```

✔ This method sets CardLayout as the layout manager for the container.

3. Methods of CardLayout

   - first(Container parent) Displays the first card.
   - last(Container parent) Displays the last card.
   - next(Container parent) Moves to the next card.
   - previous(Container parent) Moves to the previous card.
   - show(Container parent, String name) Displays the card with the specified name.

4. Example Program Using CardLayout
   ✅ Java Program to Demonstrate CardLayout

   ```java
   import java.awt._;
   import java.awt.event._;
   import javax.swing.\*;

   public class CardLayoutExample extends JFrame implements ActionListener {
   CardLayout card;
   JPanel panel;
   JButton next, prev;

       public CardLayoutExample() {
           card = new CardLayout();
           panel = new JPanel();
           panel.setLayout(card);

           // Adding cards (panels with labels)
           panel.add(new JLabel("Card 1 - Home"), "Home");
           panel.add(new JLabel("Card 2 - Settings"), "Settings");
           panel.add(new JLabel("Card 3 - About"), "About");

           // Buttons to navigate cards
           next = new JButton("Next");
           prev = new JButton("Previous");

           next.addActionListener(this);
           prev.addActionListener(this);

           add(panel, BorderLayout.CENTER);
           add(next, BorderLayout.EAST);
           add(prev, BorderLayout.WEST);

           setSize(400, 200);
           setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
           setVisible(true);
       }

       public void actionPerformed(ActionEvent e) {
           if (e.getSource() == next) {
               card.next(panel);
           } else {
               card.previous(panel);
           }
       }

       public static void main(String[] args) {
           new CardLayoutExample();
       }

   }
   ```

   ✅ Output:  
    ✔ The program displays three "cards" (Home, Settings, About).  
    ✔ Clicking "Next" moves to the next card, and "Previous" moves back.

5. Key Points for 5 Marks Answer  
   ✅ CardLayout is used to switch between multiple components (like cards).  
   ✅ Useful for tabbed interfaces, wizards, and multi-step forms.  
   ✅ Key methods: next(), previous(), first(), last(), show().  
   ✅ Example program demonstrating CardLayout navigation.  
   ✅ It improves user experience by organizing content efficiently.

---

### 6. Explain any 5 listener interface ?

1. What are Listener Interfaces?  
   ✔ In Java, Listener Interfaces are used for handling events in GUI applications.  
   ✔ They are part of the java.awt.event package.  
   ✔ Each listener interface has methods that respond to specific user actions, such as clicking a button or pressing a key.

2. Five Important Listener Interfaces

- Listener Interface Description
- ActionListener Handles button clicks and menu item selections.
- MouseListener Detects mouse clicks, entering, exiting, pressing, and releasing.
- KeyListener Captures key press, release, and typing events.
- WindowListener Monitors window events like open, close, minimize, and maximize.
- ItemListener Handles checkbox and list item selection changes.

3. Example Program Using ActionListener
   ✅ Java Program for Button Click Event

    ```java
    import java.awt._;
    import java.awt.event._;
    import javax.swing.\*;

    public class ListenerExample extends JFrame implements ActionListener {
    JButton button;

        public ListenerExample() {
            button = new JButton("Click Me");
            button.addActionListener(this); // Registering ActionListener
            add(button);
            setSize(300, 200);
            setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
            setVisible(true);
        }

        public void actionPerformed(ActionEvent e) {
            System.out.println("Button Clicked!");
        }

        public static void main(String[] args) {
            new ListenerExample();
        }

    }
    ```
✅ Output:  
✔ When the button is clicked, the message "Button Clicked!" appears in the console.

4. Key Points for 5 Marks Answer  
   ✅ Listener interfaces handle different user interactions in Java GUI.  
   ✅ Five important listener interfaces: ActionListener, MouseListener, KeyListener, WindowListener, ItemListener.  
   ✅ Each interface has methods to handle specific actions like button clicks, mouse clicks, key presses, etc.  
   ✅ Example program using ActionListener.  
   ✅ Listeners improve user interactivity in GUI applications.  

---

7. State the us of <applet> tag to build the applet?    

✔ The <applet> tag is an HTML tag used to embed Java applets in a webpage.  
✔ It loads and runs a Java applet inside a web browser.  
✔ This tag is part of older HTML versions and is now deprecated in modern browsers.

2. Syntax of <applet> Tag 

```html
<applet code="MyApplet.class" width="300" height="200"></applet>
```

✔ code: Specifies the name of the compiled Java applet file (.class).   
✔ width: Defines the width of the applet display area.   
✔ height: Defines the height of the applet display area.   

3. Example Program Using <applet>
   ✅ Java Applet Code (MyApplet.java)

```java
import java.applet.Applet;
import java.awt.Graphics;

public class MyApplet extends Applet {
 public void paint(Graphics g) {
 g.drawString("Hello, This is a Java Applet!", 50, 100);
 }
}
```

✅ HTML Code to Run the Applet (index.html)

```html
<html>
  <body>
    <applet code="MyApplet.class" width="400" height="200"></applet>
  </body>
</html>
```

✔ When the HTML file is opened in a browser that supports Java, it displays "Hello, This is a Java Applet!".

4. Attributes of <applet> Tag
   Attribute Description
   - code Specifies the Java class file of the applet.
   - width Defines the width of the applet display.
   - height Defines the height of the applet display.
   - archive Specifies a JAR file that contains the applet.
   - alt Alternative text if the browser does not support applets.
5. Key Points for 5 Marks Answer  
   ✅ The <applet> tag is used in HTML to display Java applets in a webpage.  
   ✅ It requires a compiled Java class file (.class).  
   ✅ Important attributes: code, width, height, archive, alt.  
   ✅ Example program demonstrating applet execution.  
   ✅ Now deprecated in modern browsers, replaced by JavaScript and other technologies.
---
