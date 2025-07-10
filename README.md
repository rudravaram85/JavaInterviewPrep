                                 
                                 
                                 
                                 Java Classes, Methods, Fields and Constructors Interview Questions and Answers
Absolutely! Below is a comprehensive list of **25 Java Interview Questions and Answers**, each paired with a **real-world use case coding example**, covering **Classes, Methods, Fields, and Constructors** in Java.

---

## ✅ Java Interview Questions and Answers with Examples

**Topic: Java Classes, Methods, Fields, and Constructors**

---

### 🔸 SECTION 1: **Java Classes and Fields** (Q1–Q10)

---

### **1. What is a class in Java?**

**Answer:**
A class is a blueprint for creating objects. It defines fields and methods.

**Example:**

```java
class Car {
    String brand;
    int speed;
}
```

---

### **2. What is an object in Java?**

**Answer:**
An object is an instance of a class.

**Example:**

```java
Car myCar = new Car();
myCar.brand = "Toyota";
myCar.speed = 100;
```

---

### **3. What are fields in a class?**

**Answer:**
Fields (also called variables) store the state of an object.

**Example:**

```java
class Student {
    String name;
    int rollNumber;
}
```

---

### **4. What is the difference between instance and static fields?**

**Answer:**

* **Instance fields** belong to objects.
* **Static fields** belong to the class.

**Example:**

```java
class Employee {
    String name; // instance field
    static String company = "TechCorp"; // static field
}
```

---

### **5. How do you encapsulate fields in Java?**

**Answer:**
By making fields `private` and accessing them via `getters/setters`.

**Example:**

```java
class BankAccount {
    private double balance;

    public double getBalance() {
        return balance;
    }

    public void deposit(double amount) {
        balance += amount;
    }
}
```

---

### **6. What are access modifiers in Java?**

**Answer:**
Access modifiers define the visibility of classes and members. (e.g., `public`, `private`, `protected`, default)

**Example:**

```java
public class User {
    private String password; // only accessible within the class
}
```

---

### **7. Can you define multiple classes in one file?**

**Answer:**
Yes, but only one public class is allowed per file.

**Example:**

```java
public class Main {}
class Helper {}
```

---

### **8. What is the default value of a field in Java?**

**Answer:**
Numeric types → 0, boolean → false, reference types → null.

**Example:**

```java
class Demo {
    int x; // default 0
    boolean flag; // default false
}
```

---

### **9. Can fields be final?**

**Answer:**
Yes, `final` fields cannot be changed once assigned.

**Example:**

```java
class Constants {
    final int MAX_USERS = 100;
}
```

---

### **10. What is the use of `this` keyword?**

**Answer:**
Used to refer to the current instance.

**Example:**

```java
class Person {
    String name;

    Person(String name) {
        this.name = name;
    }
}
```

---

### 🔸 SECTION 2: **Java Methods** (Q11–Q17)

---

### **11. What is a method in Java?**

**Answer:**
A method is a block of code that performs an action.

**Example:**

```java
class Calculator {
    int add(int a, int b) {
        return a + b;
    }
}
```

---

### **12. What is method overloading?**

**Answer:**
Defining multiple methods with the same name but different parameters.

**Example:**

```java
class Printer {
    void print(String s) {
        System.out.println(s);
    }

    void print(int i) {
        System.out.println(i);
    }
}
```

---

### **13. What is the return type of a method?**

**Answer:**
It specifies what the method returns (e.g., `void`, `int`, `String`).

**Example:**

```java
String getName() {
    return "John";
}
```

---

### **14. Can a method return an object?**

**Answer:**
Yes.

**Example:**

```java
class Product {
    String name;

    Product getProduct() {
        Product p = new Product();
        p.name = "Laptop";
        return p;
    }
}
```

---

### **15. What are static methods?**

**Answer:**
They belong to the class and can be called without creating an object.

**Example:**

```java
class Utility {
    static void greet() {
        System.out.println("Hello!");
    }
}
```

---

### **16. What are varargs in methods?**

**Answer:**
Variable-length arguments (`...`) allow passing multiple arguments of the same type.

**Example:**

```java
class Sum {
    int add(int... nums) {
        int total = 0;
        for (int num : nums) total += num;
        return total;
    }
}
```

---

### **17. Can methods be private?**

**Answer:**
Yes. Private methods are accessible only within the class.

**Example:**

```java
class Secure {
    private void validate() {
        System.out.println("Validating...");
    }
}
```

---

### 🔸 SECTION 3: **Java Constructors** (Q18–Q25)

---

### **18. What is a constructor in Java?**

**Answer:**
A constructor initializes an object. It has no return type and the same name as the class.

**Example:**

```java
class Book {
    String title;

    Book(String title) {
        this.title = title;
    }
}
```

---

### **19. What is constructor overloading?**

**Answer:**
Multiple constructors with different parameter lists.

**Example:**

```java
class Rectangle {
    Rectangle() {}
    Rectangle(int width, int height) {}
}
```

---

### **20. What is a default constructor?**

**Answer:**
A no-arg constructor provided by Java if no other constructors exist.

**Example:**

```java
class Sample {
    // Java automatically provides: Sample() {}
}
```

---

### **21. Can constructors be private?**

**Answer:**
Yes. Used in Singleton or Factory patterns.

**Example:**

```java
class Config {
    private Config() {}

    static Config getInstance() {
        return new Config();
    }
}
```

---

### **22. What is the use of `super()` in constructors?**

**Answer:**
To call the superclass constructor.

**Example:**

```java
class Animal {
    Animal(String name) {}
}

class Dog extends Animal {
    Dog() {
        super("Dog");
    }
}
```

---

### **23. What happens if you don't define a constructor?**

**Answer:**
Java provides a default no-arg constructor.

---

### **24. Can a constructor call another constructor?**

**Answer:**
Yes, using `this()`.

**Example:**

```java
class Box {
    int volume;

    Box() {
        this(1, 1, 1);
    }

    Box(int l, int w, int h) {
        volume = l * w * h;
    }
}
```

---

### **25. Can you overload constructors with different numbers of parameters?**

**Answer:**
Yes. This is common for providing flexible object creation.

**Example:**

```java
class User {
    String name;
    int age;

    User(String name) {
        this.name = name;
    }

    User(String name, int age) {
        this.name = name;
        this.age = age;
    }
}
```

---

Would you like this in **PDF format**, a downloadable **code workbook**, or a **flashcard-style version** for revision?


                                                              
                                                              Inheritance Interview questions

Sure! Below are **25 Java interview questions** related to **Inheritance**, each followed by a **clear answer** and a **real-world coding example** to illustrate the concept.

---

### ✅ 1. **What is inheritance in Java?**

**Answer:**
Inheritance allows a class (child) to acquire properties and methods of another class (parent). It promotes code reusability.

**Example:**

```java
class Vehicle {
    void start() {
        System.out.println("Vehicle is starting...");
    }
}

class Car extends Vehicle {
    void drive() {
        System.out.println("Car is driving...");
    }
}

public class Test {
    public static void main(String[] args) {
        Car c = new Car();
        c.start();  // Inherited from Vehicle
        c.drive();  // Own method
    }
}
```

---

### ✅ 2. **What are the types of inheritance in Java?**

**Answer:**

* Single
* Multilevel
* Hierarchical
  (Note: Java doesn’t support multiple inheritance with classes.)

**Example: Multilevel Inheritance**

```java
class Animal {
    void eat() { System.out.println("Eating..."); }
}

class Mammal extends Animal {
    void walk() { System.out.println("Walking..."); }
}

class Dog extends Mammal {
    void bark() { System.out.println("Barking..."); }
}
```

---

### ✅ 3. **Why doesn't Java support multiple inheritance with classes?**

**Answer:**
To avoid ambiguity caused by the **Diamond Problem**.

**Example (conceptual)**:

```java
class A { void show() {} }
class B { void show() {} }
// class C extends A, B {} // Compilation error due to ambiguity
```

---

### ✅ 4. **What is the `super` keyword in inheritance?**

**Answer:**
Used to access parent class methods, variables, and constructors.

**Example:**

```java
class Parent {
    int x = 10;
}

class Child extends Parent {
    int x = 20;

    void print() {
        System.out.println(super.x); // prints 10
    }
}
```

---

### ✅ 5. **Can constructors be inherited in Java?**

**Answer:**
No, but the child can call the parent constructor using `super()`.

**Example:**

```java
class Parent {
    Parent(String name) {
        System.out.println("Hello " + name);
    }
}

class Child extends Parent {
    Child() {
        super("Java");
    }
}
```

---

### ✅ 6. **What is method overriding in inheritance?**

**Answer:**
Subclasses provide a specific implementation of a method declared in a parent class.

**Example:**

```java
class Animal {
    void sound() {
        System.out.println("Animal sound");
    }
}

class Dog extends Animal {
    void sound() {
        System.out.println("Dog barks");
    }
}
```

---

### ✅ 7. **What is dynamic method dispatch?**

**Answer:**
It’s the process of resolving overridden method calls at runtime.

**Example:**

```java
Animal a = new Dog();
a.sound(); // Outputs: Dog barks
```

---

### ✅ 8. **Can a subclass override a private method?**

**Answer:**
No. Private methods are not inherited.

**Example:**

```java
class A {
    private void show() {
        System.out.println("A");
    }
}

class B extends A {
    // This is a new method, not an override
    void show() {
        System.out.println("B");
    }
}
```

---

### ✅ 9. **What is the use of protected access modifier in inheritance?**

**Answer:**
Allows access within the package and to subclasses outside the package.

**Example:**

```java
class Base {
    protected void display() {
        System.out.println("Base Display");
    }
}
```

---

### ✅ 10. **What is the output of calling a subclass object with a superclass reference?**

**Answer:**
The overridden method in the subclass is called (runtime polymorphism).

**Example:**

```java
Animal a = new Dog();
a.sound(); // Dog barks
```

---

### ✅ 11. **Can we access subclass-specific methods using superclass reference?**

**Answer:**
No, unless you cast it.

**Example:**

```java
Animal a = new Dog();
// a.bark(); // Error
((Dog)a).bark(); // Works
```

---

### ✅ 12. **How do interfaces relate to inheritance?**

**Answer:**
Interfaces allow multiple inheritance of type.

**Example:**

```java
interface Flyable {
    void fly();
}

class Bird implements Flyable {
    public void fly() {
        System.out.println("Flying");
    }
}
```

---

### ✅ 13. **Can a class extend multiple classes in Java?**

**Answer:**
No, Java doesn’t allow multiple class inheritance.

---

### ✅ 14. **Can a class implement multiple interfaces?**

**Answer:**
Yes.

**Example:**

```java
interface A { void a(); }
interface B { void b(); }

class C implements A, B {
    public void a() {}
    public void b() {}
}
```

---

### ✅ 15. **What is hierarchical inheritance?**

**Answer:**
One parent, multiple child classes.

**Example:**

```java
class Parent {}

class Child1 extends Parent {}
class Child2 extends Parent {}
```

---

### ✅ 16. **What happens if we don't call `super()` explicitly in constructor?**

**Answer:**
Java inserts `super()` implicitly.

---

### ✅ 17. **How does method resolution work in inheritance?**

**Answer:**
Starts from subclass → up the hierarchy until found.

---

### ✅ 18. **Can abstract classes participate in inheritance?**

**Answer:**
Yes. Abstract classes are often extended to implement their methods.

**Example:**

```java
abstract class Shape {
    abstract void draw();
}

class Circle extends Shape {
    void draw() {
        System.out.println("Drawing Circle");
    }
}
```

---

### ✅ 19. **Can we prevent inheritance in Java?**

**Answer:**
Yes, by declaring the class as `final`.

**Example:**

```java
final class A {}
// class B extends A {} // Compilation error
```

---

### ✅ 20. **Can we override static methods?**

**Answer:**
No, static methods belong to the class, not instance.

**Example:**

```java
class A {
    static void show() {
        System.out.println("A");
    }
}

class B extends A {
    static void show() {
        System.out.println("B");
    }
}
```

---

### ✅ 21. **What happens if subclass has constructor with more parameters?**

**Answer:**
Must explicitly call the matching parent constructor using `super()`.

---

### ✅ 22. **Can we use inheritance with packages?**

**Answer:**
Yes. Use `import` and `protected` access modifier for cross-package inheritance.

---

### ✅ 23. **What is IS-A relationship in Java?**

**Answer:**
Inheritance represents an IS-A relationship.

**Example:**
`Dog IS-A Animal` → Dog extends Animal

---

### ✅ 24. **Can constructors be overridden?**

**Answer:**
No, constructors are not inherited, hence cannot be overridden.

---

### ✅ 25. **What is object slicing in inheritance?**

**Answer:**
Not applicable in Java. Java always accesses full object (unlike C++).

---

Would you like this as a downloadable PDF or formatted Markdown for easy copy-paste into documentation or study notes?

---


                                           Java Interface Interview Questions and answers

Absolutely! Here are **25 interview questions and answers on Java Interfaces**, each with a **real-time use case coding example** to help solidify the concept:

---

### ✅ 1. **What is an interface in Java?**

**Answer:**
An interface is a reference type in Java, similar to a class, that can contain **only constants, method signatures, default methods, static methods**, and **nested types**. It is used to **achieve abstraction and multiple inheritance**.

**Real-time Example:**

```java
interface PaymentGateway {
    void processPayment(double amount);
}

class PayPal implements PaymentGateway {
    public void processPayment(double amount) {
        System.out.println("Paid $" + amount + " via PayPal");
    }
}
```

---

### ✅ 2. **Can an interface have method implementations in Java?**

**Answer:**
Yes, Java 8 introduced **default** and **static** methods with implementation inside interfaces.

**Example:**

```java
interface Vehicle {
    default void start() {
        System.out.println("Vehicle is starting");
    }
}
```

---

### ✅ 3. **How do you implement multiple interfaces in Java?**

**Answer:**
Use a comma-separated list in the class declaration.

**Example:**

```java
interface GPS {
    void locate();
}

interface Camera {
    void takePhoto();
}

class Smartphone implements GPS, Camera {
    public void locate() { System.out.println("Locating using GPS..."); }
    public void takePhoto() { System.out.println("Photo taken!"); }
}
```

---

### ✅ 4. **What is the difference between abstract class and interface?**

**Answer:**

| Abstract Class        | Interface                 |
| --------------------- | ------------------------- |
| Can have constructors | Cannot have constructors  |
| Can maintain state    | Cannot maintain state     |
| Partial abstraction   | Full abstraction (mostly) |

---

### ✅ 5. **What is the use of default methods in interfaces?**

**Answer:**
To add new methods to interfaces without breaking existing implementations.

**Example:**

```java
interface Logger {
    default void log(String msg) {
        System.out.println("Log: " + msg);
    }
}
```

---

### ✅ 6. **Can interfaces extend other interfaces?**

**Answer:**
Yes, an interface can extend one or more other interfaces.

**Example:**

```java
interface Movable {
    void move();
}

interface Flyable extends Movable {
    void fly();
}
```

---

### ✅ 7. **Can a class implement two interfaces with the same method signature?**

**Answer:**
Yes, and only **one implementation** is required.

**Example:**

```java
interface A { void show(); }
interface B { void show(); }

class C implements A, B {
    public void show() {
        System.out.println("Common show()");
    }
}
```

---

### ✅ 8. **Can we declare variables in interfaces?**

**Answer:**
Yes, but they are **implicitly public, static, and final**.

**Example:**

```java
interface Config {
    int MAX_USERS = 100; // constant
}
```

---

### ✅ 9. **Can an interface be instantiated?**

**Answer:**
No. Interfaces **cannot be instantiated** directly.

```java
// Invalid: PaymentGateway pg = new PaymentGateway();
```

---

### ✅ 10. **What is marker interface in Java?**

**Answer:**
An interface with **no methods**, used to mark or signal something.

**Example:**

```java
interface Serializable {}

class User implements Serializable {
    // Signals to JVM this object can be serialized
}
```

---

### ✅ 11. **What happens if two interfaces have default methods with the same signature?**

**Answer:**
The class must override the method to resolve conflict.

**Example:**

```java
interface A {
    default void hello() { System.out.println("Hello A"); }
}

interface B {
    default void hello() { System.out.println("Hello B"); }
}

class C implements A, B {
    public void hello() {
        System.out.println("Conflict resolved in C");
    }
}
```

---

### ✅ 12. **Can an interface contain constructors?**

**Answer:**
No. Interfaces cannot have constructors because they can’t be instantiated.

---

### ✅ 13. **What is functional interface?**

**Answer:**
An interface with **only one abstract method** (Java 8 feature). Enables lambda expressions.

**Example:**

```java
@FunctionalInterface
interface Greeter {
    void greet(String name);
}
```

---

### ✅ 14. **What is SAM Interface?**

**Answer:**
**Single Abstract Method interface** — same as functional interface.

---

### ✅ 15. **Can interfaces have static methods?**

**Answer:**
Yes, since Java 8.

**Example:**

```java
interface MathUtils {
    static int square(int x) {
        return x * x;
    }
}
```

---

### ✅ 16. **How do you achieve abstraction using interfaces?**

**Answer:**
By only exposing method signatures, hiding the implementation.

**Example:**

```java
interface Printer {
    void print(String doc);
}

class PDFPrinter implements Printer {
    public void print(String doc) {
        System.out.println("Printing PDF: " + doc);
    }
}
```

---

### ✅ 17. **Can interfaces extend multiple interfaces?**

**Answer:**
Yes.

**Example:**

```java
interface A {}
interface B {}
interface C extends A, B {}
```

---

### ✅ 18. **What if a class does not implement all methods of an interface?**

**Answer:**
The class must be declared `abstract`.

---

### ✅ 19. **Can you implement interface methods as private?**

**Answer:**
No, interface methods are **implicitly public**, so implementations must be public.

---

### ✅ 20. **Can we have inner interfaces in Java?**

**Answer:**
Yes. They are implicitly `static`.

**Example:**

```java
class Outer {
    interface Inner {
        void show();
    }
}
```

---

### ✅ 21. **Can interfaces be generic?**

**Answer:**
Yes.

**Example:**

```java
interface Repository<T> {
    void save(T obj);
}
```

---

### ✅ 22. **What is a real-time use of interface in Java frameworks?**

**Answer:**
In Spring, interfaces are used for **loose coupling**.

**Example:**

```java
interface NotificationService {
    void send(String msg);
}

class EmailService implements NotificationService {
    public void send(String msg) {
        System.out.println("Sending Email: " + msg);
    }
}
```

---

### ✅ 23. **How are interfaces used in Dependency Injection?**

**Answer:**
Interfaces allow injecting different implementations at runtime.

**Example with constructor injection:**

```java
class OrderService {
    private final PaymentGateway pg;

    OrderService(PaymentGateway pg) {
        this.pg = pg;
    }

    void checkout() {
        pg.processPayment(200);
    }
}
```

---

### ✅ 24. **Can you override interface methods in implementing class?**

**Answer:**
Yes, all abstract methods must be overridden.

---

### ✅ 25. **Can interface methods throw exceptions?**

**Answer:**
Yes, method signatures can declare exceptions.

**Example:**

```java
interface FileReader {
    void read(String path) throws IOException;
}
```

---

Would you like these questions in a **PDF format** or **interactive quiz form**?
                                           



Would you like a downloadable `.docx` file instead?


                                      Java Exception Handling Interview Questions and Answers

---

## ✅ 25 Java Exception Handling Interview Questions & Answers

### Focus: `try`, `catch`, `finally`

---

### 🔹 **Basic Level (1–10)**

---

1. **What is exception handling in Java?**
   ➤ Exception handling is the process of handling runtime errors using constructs like `try`, `catch`, `throw`, `throws`, and `finally`.

---

2. **What is an exception?**
   ➤ An exception is an object that represents an error or unexpected condition during program execution.

---

3. **What is the purpose of `try` block?**
   ➤ The `try` block is used to wrap code that might throw exceptions.

---

4. **What is the purpose of `catch` block?**
   ➤ A `catch` block handles specific exceptions thrown within the associated `try` block.

---

5. **What is the purpose of the `finally` block?**
   ➤ The `finally` block contains code that **always executes** after the `try` block, regardless of whether an exception was thrown or caught.

---

6. **Can a `try` block exist without a `catch` block?**
   ➤ Yes, but only if a `finally` block is present.

```java
try {
   // risky code
} finally {
   // cleanup code
}
```

---

7. **Can a `catch` block exist without a `try` block?**
   ➤ No. A `catch` must always be associated with a `try`.

---

8. **What happens if an exception is not caught?**
   ➤ The program terminates abnormally and the JVM prints the stack trace.

---

9. **Can multiple `catch` blocks be used with a single `try` block?**
   ➤ Yes. Each `catch` block handles a different exception type.

---

10. **In what order are `catch` blocks checked?**
    ➤ From top to bottom. More specific exceptions should be caught before more general ones.

---

### 🔹 **Intermediate Level (11–20)**

---

11. **What happens if the `finally` block throws an exception?**
    ➤ It overrides any exception thrown in the `try` or `catch` block.

---

12. **Is the `finally` block always executed?**
    ➤ Yes, except when the JVM exits using `System.exit()` or the thread is killed.

---

13. **Can a `try` block be nested?**
    ➤ Yes. Java supports nested `try-catch` blocks.

---

14. **What is exception propagation?**
    ➤ It refers to the process of passing the exception from one method to another up the call stack until it is caught.

---

15. **Can we use multiple exceptions in a single `catch` block?**
    ➤ Yes, from Java 7 onward using multi-catch:

```java
catch (IOException | SQLException e) {
   e.printStackTrace();
}
```

---

16. **What is the difference between checked and unchecked exceptions?**
    ➤ **Checked exceptions** must be handled or declared (e.g., `IOException`).
    ➤ **Unchecked exceptions** are not required to be handled (e.g., `NullPointerException`).

---

17. **Can we rethrow an exception from a `catch` block?**
    ➤ Yes, using the `throw` keyword.

---

18. **Can a `finally` block modify the return value from a `try` block?**
    ➤ Yes, if the return statement is in both blocks, the one in `finally` will override it.

---

19. **Can `return` be used in `try`, `catch`, and `finally` blocks?**
    ➤ Yes, but using `return` in `finally` can lead to unexpected behavior and should be avoided.

---

20. **Can we catch the base class `Exception` instead of specific ones?**
    ➤ Yes, but it's best practice to catch specific exceptions when possible.

---

### 🔹 **Advanced Level (21–25)**

---

21. **What happens if both `catch` and `finally` blocks throw exceptions?**
    ➤ The exception in the `finally` block will **suppress** the one in the `catch` block.

---

22. **How to ensure resource cleanup when an exception occurs?**
    ➤ Use `finally` blocks or Java 7’s **try-with-resources** for `AutoCloseable` resources.

---

23. **Is it a good practice to catch `Exception` or `Throwable`?**
    ➤ Generally no, unless you're writing top-level error handlers or logging frameworks.

---

24. **Can exceptions be caught and ignored?**
    ➤ Yes, but it’s considered bad practice unless you document a valid reason.

```java
try {
   riskyOperation();
} catch (Exception e) {
   // ignored
}
```

---

25. **What are common runtime exceptions that can be caught using `catch` blocks?**
    ➤ Examples:

* `NullPointerException`
* `ArrayIndexOutOfBoundsException`
* `ArithmeticException`
* `IllegalArgumentException`

---

Would you like these questions as a **PDF**, **quiz**, or in **flashcard format** for studying?

                                                       Java Collections and Wrapper Classes Interview Questions and Answers


Absolutely! Below are **25 Java Interview Questions and Answers**, each accompanied by a **real-world use case coding example**, focused on **Java Collections and Wrapper Classes**.

---

## ✅ Java Interview Questions & Answers: Collections and Wrapper Classes

Each answer includes a **real-world coding example** to help reinforce the concept.

---

### 🔹 SECTION 1: **Java Collections** (1–15)

---

### **1. What is the Java Collections Framework?**

**Answer:**
It is a set of classes and interfaces that implement commonly reusable data structures such as Lists, Sets, Maps, and Queues.

**Example:**

```java
import java.util.*;

public class ProductCatalog {
    public static void main(String[] args) {
        List<String> products = new ArrayList<>();
        products.add("Laptop");
        products.add("Mouse");
        products.add("Keyboard");

        System.out.println("Available Products:");
        products.forEach(System.out::println);
    }
}
```

---

### **2. What is the difference between List, Set, and Map?**

**Answer:**

* `List`: Ordered, allows duplicates
* `Set`: Unordered, no duplicates
* `Map`: Key-value pairs, keys unique

**Example:**

```java
import java.util.*;

public class CollectionTypesDemo {
    public static void main(String[] args) {
        List<String> list = Arrays.asList("A", "B", "A");
        Set<String> set = new HashSet<>(list);
        Map<Integer, String> map = Map.of(1, "Apple", 2, "Banana");

        System.out.println("List (allows duplicates): " + list);
        System.out.println("Set (no duplicates): " + set);
        System.out.println("Map (key-value): " + map);
    }
}
```

---

### **3. What is the default capacity of an `ArrayList`?**

**Answer:**
The default capacity is 10.

**Example:**

```java
List<String> cities = new ArrayList<>();
cities.add("New York");
cities.add("London");
// Capacity expands automatically as items are added
```

---

### **4. How is `LinkedList` different from `ArrayList`?**

**Answer:**
`LinkedList` is better for frequent insertions/deletions; `ArrayList` is better for random access.

**Example:**

```java
List<String> linkedList = new LinkedList<>();
linkedList.add("Item1");
linkedList.add(0, "Item0");
System.out.println(linkedList);
```

---

### **5. What is a `HashSet` and when would you use it?**

**Answer:**
It’s used to store unique elements without any specific order.

**Example:**

```java
Set<String> emails = new HashSet<>();
emails.add("a@example.com");
emails.add("b@example.com");
emails.add("a@example.com"); // Duplicate

System.out.println("Unique Emails: " + emails);
```

---

### **6. How do you sort a list of names alphabetically?**

**Answer:**

```java
List<String> names = Arrays.asList("Zoe", "Alice", "Bob");
Collections.sort(names);
System.out.println("Sorted Names: " + names);
```

---

### **7. What is `LinkedHashSet`?**

**Answer:**
Maintains insertion order and disallows duplicates.

**Example:**

```java
Set<String> orderedSet = new LinkedHashSet<>();
orderedSet.add("One");
orderedSet.add("Two");
orderedSet.add("One"); // Duplicate
System.out.println(orderedSet); // Preserves order
```

---

### **8. What is `TreeSet` used for?**

**Answer:**
It stores elements in **sorted order**.

**Example:**

```java
Set<Integer> numbers = new TreeSet<>(Arrays.asList(5, 3, 1, 4, 2));
System.out.println("Sorted Numbers: " + numbers);
```

---

### **9. What is the difference between `HashMap` and `TreeMap`?**

**Answer:**

* `HashMap`: Unordered, faster
* `TreeMap`: Sorted by keys

**Example:**

```java
Map<String, Integer> treeMap = new TreeMap<>();
treeMap.put("Banana", 3);
treeMap.put("Apple", 2);
treeMap.put("Orange", 5);
System.out.println(treeMap); // Sorted by key
```

---

### **10. How to safely iterate and remove from a collection?**

**Answer:**
Use an iterator to avoid `ConcurrentModificationException`.

**Example:**

```java
List<String> names = new ArrayList<>(Arrays.asList("Tom", "Tim", "Tam"));
Iterator<String> it = names.iterator();
while (it.hasNext()) {
    if (it.next().startsWith("T")) {
        it.remove();
    }
}
System.out.println(names); // []
```

---

### **11. What is `Collections.unmodifiableList()` used for?**

**Answer:**
To create a read-only list.

**Example:**

```java
List<String> modifiable = new ArrayList<>(List.of("A", "B"));
List<String> unmodifiable = Collections.unmodifiableList(modifiable);
// unmodifiable.add("C"); // Throws exception
```

---

### **12. What is the purpose of `Collections.sort()`?**

**Answer:**
To sort lists in natural or custom order.

**Example:**

```java
List<Integer> numbers = Arrays.asList(4, 2, 1, 3);
Collections.sort(numbers);
System.out.println(numbers);
```

---

### **13. What is `Queue` in Java used for?**

**Answer:**
To model FIFO (First-In-First-Out) structures like task scheduling.

**Example:**

```java
Queue<String> tasks = new LinkedList<>();
tasks.add("Download");
tasks.add("Process");
System.out.println(tasks.poll()); // Download
```

---

### **14. How does `ConcurrentHashMap` help in multithreading?**

**Answer:**
It is a thread-safe alternative to `HashMap`.

**Example:**

```java
Map<String, Integer> stock = new ConcurrentHashMap<>();
stock.put("Apples", 50);
stock.compute("Apples", (k, v) -> v - 10);
```

---

### **15. How can you convert a List to a Set?**

**Answer:**

```java
List<String> list = Arrays.asList("A", "B", "A");
Set<String> set = new HashSet<>(list);
System.out.println(set); // [A, B]
```

---

### 🔹 SECTION 2: **Wrapper Classes** (16–25)

---

### **16. What are wrapper classes?**

**Answer:**
Object versions of primitive types.

**Example:**

```java
int a = 5;
Integer aObj = a; // Autoboxing
```

---

### **17. What is autoboxing and unboxing?**

**Answer:**

* **Autoboxing**: `int` to `Integer`
* **Unboxing**: `Integer` to `int`

**Example:**

```java
Integer num = 10;  // Autoboxing
int value = num;   // Unboxing
```

---

### **18. Why do we need wrapper classes in collections?**

**Answer:**
Collections can only store objects, not primitives.

**Example:**

```java
List<Integer> numbers = new ArrayList<>();
numbers.add(10); // Autoboxes primitive int
```

---

### **19. Are wrapper classes immutable?**

**Answer:**
Yes, like `String`, wrapper classes are immutable.

**Example:**

```java
Integer a = 10;
Integer b = a;
a = 20;
System.out.println(b); // 10
```

---

### **20. How to convert a String to a primitive using wrapper classes?**

**Answer:**

```java
String price = "100";
int p = Integer.parseInt(price);
```

---

### **21. Can you store `null` in wrapper classes?**

**Answer:**
Yes.

**Example:**

```java
Integer count = null;
System.out.println(count); // null
```

---

### **22. What is the default value of wrapper class fields?**

**Answer:**
`null` for wrapper objects.

---

### **23. How do you compare wrapper class values correctly?**

**Answer:**

```java
Integer x = 128;
Integer y = 128;
System.out.println(x.equals(y)); // true
System.out.println(x == y);      // false
```

---

### **24. What utility methods are available in wrapper classes?**

**Answer:**
Parsing, comparing, etc.

**Example:**

```java
int max = Integer.max(10, 20);
```

---

### **25. How do wrapper classes support caching?**

**Answer:**
`Integer` caches values from -128 to 127 for performance.

**Example:**

```java
Integer a = 100;
Integer b = 100;
System.out.println(a == b); // true
```

---

Would you like this as a **PDF**, or want a separate file with **only code snippets** for practice?

                                                       

