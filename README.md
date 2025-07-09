                                 
                                 
                                 
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

I can’t directly copy text to your clipboard, but you can easily do it yourself:

Here’s the full content ready to **select and copy**:

---

### ✅ **25 Java Inheritance Interview Questions and Answers**

#### 🔹 Basic Level (1–10)

1. **What is inheritance in Java?**
   ➤ Inheritance is an OOP feature that allows a class (child/subclass) to inherit properties and behaviors (fields and methods) from another class (parent/superclass).

2. **What are the types of inheritance supported by Java?**
   ➤ Java supports:

   * Single Inheritance
   * Multilevel Inheritance
   * Hierarchical Inheritance
     ➤ Java does not support multiple inheritance with classes directly but does through interfaces.

3. **Why is multiple inheritance not supported in Java with classes?**
   ➤ To avoid ambiguity and complexity like the Diamond Problem. Java uses interfaces to resolve such issues.

4. **What is the difference between `extends` and `implements`?**
   ➤ `extends` is used to inherit from a class.
   ➤ `implements` is used to inherit from an interface.

5. **Can constructors be inherited?**
   ➤ No. Constructors are not inherited, but can be called via `super()`.

6. **What is the use of the `super` keyword?**
   ➤ Used to access the superclass constructor, methods, or variables.

7. **What is method overriding?**
   ➤ A subclass providing its own implementation of a method defined in its superclass.

8. **What is the difference between overloading and overriding?**
   ➤ **Overloading**: Same method name, different parameters.
   ➤ **Overriding**: Same method signature, subclass redefines it.

9. **Can private methods be overridden?**
   ➤ No. They are not visible to the subclass.

10. **Can a subclass access private members of a superclass?**
    ➤ No. Only via public/protected methods if provided.

---

#### 🔹 Intermediate Level (11–20)

11. **What is dynamic method dispatch?**
    ➤ A mechanism where a call to an overridden method is resolved at runtime.

12. **Can final methods be overridden?**
    ➤ No. Final methods cannot be overridden.

13. **Can static methods be overridden?**
    ➤ No. They are hidden, not overridden.

14. **What happens if a subclass constructor does not call `super()` explicitly?**
    ➤ Java inserts a call to the superclass’s no-arg constructor. If it doesn't exist, a compilation error occurs.

15. **Can a subclass override a method with a more restrictive access modifier?**
    ➤ No. The access level must be the same or more accessible.

16. **How can you prevent a class from being subclassed?**
    ➤ Declare it as `final`.

17. **What happens when a subclass has the same method as a superclass and you call it via the superclass reference?**
    ➤ The subclass’s version runs — runtime polymorphism.

18. **Can an abstract class have constructors?**
    ➤ Yes.

19. **What is the default access modifier of a class?**
    ➤ Package-private.

20. **Is it possible to call a superclass method from the subclass?**
    ➤ Yes, using `super.methodName()`.

---

#### 🔹 Advanced Level (21–25)

21. **What happens if two interfaces implemented by a class have the same method signature?**
    ➤ One implementation is enough.

22. **How does Java resolve the diamond problem with interfaces?**
    ➤ The implementing class must override the conflicting method explicitly.

23. **Can you inherit both a class and an interface in Java?**
    ➤ Yes.

24. **What are the limitations of inheritance?**
    ➤ Tight coupling, less flexibility.

25. **When should you prefer composition over inheritance?**
    ➤ When you want more flexibility or change behavior at runtime (`has-a` relationship).

---

                                                        Interfaces interview questions

Sure! Here's a comprehensive list of **25 Java Interview Questions and Answers on Interfaces**, covering **basic to advanced levels**.

---

## ✅ 25 Java Interface Interview Questions and Answers

### 🔹 **Basic Level (1–10)**

---

1. **What is an interface in Java?**
   ➤ An interface is a reference type in Java, similar to a class, that can contain only constants, method signatures, default methods, static methods, and nested types. Interfaces cannot be instantiated and are used to specify a contract that classes must implement.

---

2. **How is an interface different from an abstract class?**
   ➤ Key differences:

   * Interfaces support multiple inheritance, abstract classes don’t.
   * Abstract classes can have constructors and instance variables; interfaces can’t (except constants).
   * Interfaces are fully abstract (until Java 7); from Java 8, they can have default and static methods.

---

3. **Can an interface contain method implementations in Java?**
   ➤ Yes, from Java 8 onward, interfaces can have:

   * **Default methods** (with `default` keyword)
   * **Static methods**

---

4. **What are default methods in interfaces?**
   ➤ A `default` method is a method with a body in an interface. It allows the interface to provide a default implementation without breaking existing classes.

---

5. **What are static methods in interfaces?**
   ➤ Static methods belong to the interface itself and are not inherited by implementing classes. They must be called using the interface name.

---

6. **Can interfaces have constructors?**
   ➤ No. Interfaces cannot have constructors because they cannot be instantiated.

---

7. **Can we create an object of an interface?**
   ➤ No. Interfaces cannot be instantiated directly. You must implement them in a class and instantiate that class.

---

8. **Can an interface extend another interface?**
   ➤ Yes. An interface can extend one or more other interfaces using the `extends` keyword.

---

9. **Can a class implement multiple interfaces?**
   ➤ Yes. A class can implement multiple interfaces, which is Java’s way of supporting multiple inheritance.

---

10. **What is the syntax for implementing an interface in a class?**

```java
interface MyInterface {
    void show();
}

class MyClass implements MyInterface {
    public void show() {
        System.out.println("Implementation");
    }
}
```

---

### 🔹 **Intermediate Level (11–20)**

---

11. **Can an interface extend multiple interfaces?**
    ➤ Yes. Interfaces can extend multiple other interfaces.

```java
interface A {}
interface B {}
interface C extends A, B {}
```

---

12. **Can an interface have variables?**
    ➤ Yes, but they are implicitly `public`, `static`, and `final` (i.e., constants).

---

13. **What is the default access modifier for methods in interfaces?**
    ➤ Prior to Java 9: `public abstract`.
    ➤ Java 8+ can also have `default` and `static`.
    ➤ Java 9+ allows `private` methods inside interfaces.

---

14. **What happens if a class does not implement all methods of an interface?**
    ➤ It must be declared `abstract`. Otherwise, a compile-time error occurs.

---

15. **Can we use access modifiers with interface methods?**
    ➤ Yes, but only `public`, `default`, `private`, and `static` (Java 8+).

---

16. **Can a class both extend a class and implement an interface?**
    ➤ Yes. Java allows:

```java
class MyClass extends SuperClass implements MyInterface {}
```

---

17. **What is a functional interface?**
    ➤ An interface with **exactly one abstract method**. It can have multiple default or static methods.

---

18. **What is the purpose of `@FunctionalInterface` annotation?**
    ➤ It marks an interface as functional and helps the compiler report an error if the interface contains more than one abstract method.

---

19. **What are marker interfaces in Java?**
    ➤ Interfaces with no methods or fields, used to "mark" a class for special behavior.
    **Examples**: `Serializable`, `Cloneable`.

---

20. **How do interfaces support multiple inheritance in Java?**
    ➤ A class can implement multiple interfaces, allowing it to inherit behaviors from multiple sources, thus achieving multiple inheritance.

---

### 🔹 **Advanced Level (21–25)**

---

21. **How is a conflict resolved when a class implements two interfaces with the same default method?**
    ➤ The implementing class must **override** the conflicting method to resolve ambiguity.

---

22. **Can we override interface static methods in implementing classes?**
    ➤ No. Static methods in interfaces are not inherited by implementing classes, hence cannot be overridden.

---

23. **Can we define private methods in interfaces?**
    ➤ Yes, from Java 9 onward. Private methods can be used to share code between default and static methods within the interface.

---

24. **Why use interfaces when abstract classes can serve similar purposes?**
    ➤ Interfaces promote loose coupling, support multiple inheritance, and are ideal for defining APIs and contracts in large systems.

---

25. **How are interfaces used in real-time applications?**
    ➤ Interfaces are used to:

* Define **contracts** in frameworks (e.g., `List`, `Map`, `Runnable`).
* Enable **dependency injection** and **loose coupling** in Spring.
* Support **polymorphism** in design patterns like **Strategy** and **Observer**.

---

Would you like this formatted as a **PDF** or **Quiz** or saved for later use?
                                                        

Once copied, you can paste it into a Word processor, notes app, or an online PDF generator like [pdfcrowd.com](https://www.pdfcrowd.com/) or [web2pdfconvert.com](https://web2pdfconvert.com/).

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

                                                       

