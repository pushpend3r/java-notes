A variable is the name given to a memory location. It is the basic unit of storage in a program.
- the value stored in the variable can be changed during the execution of the program.
- all the operations done on the variable directly effects the value in the memory location.
- In Java, all variables must be declared before use.

**Syntax -** 
```java
int name;
```

here `int` is the data type means which type of data this variable stores.
`name` is the name of the variable.

In the above code we are declaring the variable so that jvm knows it exists.

When we are just declaring the variable it gets it's value based upon the data type's default value.

Rules of naming variable names - [[Basics#Rules for defining Identifiers|here]].

So `int name;` means just declaring the variable, and `int name = "Pushpender Singh";` means declaring and as well as initializing the variable.

---

Q: What is scope of a variable?
A: The **scope** of a **variable** is the region of a program in which the **variable** is visible, i.e., in which it is accessible by its name and can be used. 

### Types
- Local Variable
- Instance Variable
- Static Variable

##### Local Variable
A variable defined in the block means between `{` and `}` and not a field of class.

 - Scope is within the block.

- Initialization is **Must** unless you will get complier error like this - 

```java
Main.java:4: error: variable a might not have been initialized
    System.out.println(a);
                       ^
1 error
```

##### Instance Variable
A non-static variable that is a field of a class.

- Scope = depending upon access specifiers.
- Can be accessed only by creating objects (instance of class).

```java
public class Student {
	String name;
}
```

##### Static Variable
A variable declared with keyword `static` and is a field of a class.

```java
public class Student {
	static String class = "12th";
}
```