# Taking Input from the user

4 Ways :-
- Using Buffered Reader Class 😥
- Using Scanner Class ✔
- Using Console Class 👏
- Using Command line argument 😐


---
---

### Using Scanner Class
This is probably the most preferred method to take input.

```java
import java.util.Scanner;

class GetInputFromUser {

 public static void main(String args[]) {
 	Scanner in = new Scanner(System.in);

 	String s = in.nextLine();
 	System.out.println("You entered string " + s);
 
 	int a = in.nextInt();
 	System.out.println("You entered integer " + a);
 
 	float b = in.nextFloat();
 	System.out.println("You entered float " + b);

 	// closing scanner
 	in.close();

 }
}
```

**Caveat -**

*Guess the output*

```java
import java.util.Scanner;
class Main
{
     public static void main(String args[])
     {
        Scanner scn = new Scanner(System.in);
        System.out.println("Enter an integer");
        int a = scn.nextInt();
        System.out.println("Enter a String");
        String b = scn.nextLine();
        System.out.printf("You have entered:- " + a + " " + "and name as " + b);
        scn.close();
     }
}
```

Input - 
```
50
Geek
```

Expected Output - 
```
Enter an integer
Enter a String
You have entered:- 50 and name as Geek
```

Actual Output - 
```
Enter an integer
Enter a String
You have entered:- 50 and name as
```

In this approach if we call `nextLine()` method after any one of the seven `next___()` method then the `nextLine()` does not read values from console and cursor will not come into console it will skip that step.

The `next___()` methods are `nextInt()`, `nextFloat()`, `nextByte()`, `nextShort()`, `nextDouble()`, `nextLong()`, `next()`.

What is happening here is that `next___()` methods leave `\n` (newline character) in the buffer. And `nextLine()` method ends the line when it found `\n` (newline character).

So when `nextLine()` starts its processing it finds `\n` in the buffer so it stops. Basically It starts and then immediately ends 😂.

---

### Using Console Class
It has been becoming a preferred way for reading user’s input from the command line.

It can be used for reading password-like input without displaying the characters entered by the user as he or she types.

```java
public class Sample {
 public static void main(String[] args)
 {
 	// Using Console to input data from user
 	String name = System.console().readLine(); 
 	System.out.println("You entered string " + name);
	
	int a = Integer.parseInt(System.console().readLine());
 	System.out.println("You entered number " + a);
 }
}
```

---