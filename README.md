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
