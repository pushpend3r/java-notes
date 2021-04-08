Operators are used to perform operations on variables and values.

There are various types of operators in Java :- 
- Arithmetic
- Unary
- Assignment
- Relational
- Logical
- Ternary
- Bitwise
- Shift
- `instance of `

#### Arithmetic
1. `*` : Multiplication - `a * b` --> multiply `a` and `b`.
2. `/` : Division - `a / b` --> divides `a` by `b`.
3. `%` : Modulo - `a % b` --> gives remainder of `a / b`.
4. `+` : Addition - `a + b` --> add `a` and `b`.
5. `-` : Subtraction - `a - b` --> sub `a` to `b`.

Note - if `a` and `b` both are `int` type then the result is also `int` type. e.g.
```java
int a = 12;
int b = 5;
int c = a / b; // c would be 2 instead of 2.4
```

#### Unary
1. `-` : Unary minus - `-a`.
2. `+` : Unary Plus - `+a` --> this is default.
	Also it performs an automatic conversion to `int` when the type of its operand is `byte`, `char`, or `short`. This is called unary numeric promotion.