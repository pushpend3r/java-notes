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
3. `++` : Increment Operator - `++a` or `a++`
	- Post Increment - `a++` - Value is first used for computing the result  and the incremented.
	```java
	int a = x++;
	// If x was 10 then a also be 10 and then x will be incremented to 11
	```
	- Pre Increment - `++a` - Value is incremented first and then used for computing the result.
	```java
	int a = ++x;
	// If x was 10, it will incremented to 11 and then value is assigned to a.
	```
4. `--`: Decremented Operator - `--a` or `a--`
	Same as Increment Operator but here value is decrement by 1.
5. `!` : Logical not Operator - `!a`
	used for inverting the boolean value, means `true` becames `false` or vice verse.

#### Assignment
`=` used to assign value to the variable. e.g.
```java
int a = 12;
```

value or expression on the right side will be assigned to right side.

Note: Expression is something that produces some value.

In many cases assignment operator can be combined with other operators to build a shorter version of statement called **Compound Statement**. For example, instead of `a = a + 5`, we can write `a += 5`.

- `+=` 
- `-=`
- `*=`
- `/=`
- `%=`

#### Relational

use to check equality, greater than, less than. It returns boolean result means either `true` or `false`.

