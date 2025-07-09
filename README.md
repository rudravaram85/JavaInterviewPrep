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

Once copied, you can paste it into a Word processor, notes app, or an online PDF generator like [pdfcrowd.com](https://www.pdfcrowd.com/) or [web2pdfconvert.com](https://web2pdfconvert.com/).

Would you like a downloadable `.docx` file instead?
