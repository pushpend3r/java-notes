Try the following:

```java
int i = 20;
float f = 20.2f;
System.out.println(((Object)i).getClass().getName());
System.out.println(((Object)f).getClass().getName());
```

It will print:

```java
java.lang.Integer
java.lang.Float
```

As for `instanceof`, you could use its dynamic counterpart [`Class#isInstance`](http://docs.oracle.com/javase/7/docs/api/java/lang/Class.html#isInstance%28java.lang.Object%29):

```java
Integer.class.isInstance(20);  // true
Integer.class.isInstance(20f); // false
Integer.class.isInstance("s"); // false
```