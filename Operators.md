Operators are used to perform operations on variables or values.

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

---

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

---

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

---

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
etc...

---

#### Relational

use to check equality, greater than, less than. It returns boolean result means either `true` or `false`.

Syntax - 

`variable relation_opertor value/expression`

- `==` : Equals To - returns `true` if left side is equal to right side
- `!=` : not equals to - returns `true` if left side is not equal to right side.
- `<` : less than
- `>` : greater than
- `<=` : less than or equals to
- `>=` : greater than or equals to

---

#### Logical
used to determine the logic between variables or values:
1. `&&` : Logical AND - returns true if both expressions are true
	```java
	boolean a = true;
	boolean b = false;
	boolean result = a && b; // false
	```
2. `||` : Logical OR - returns true if either of the expressions are true.
	```java
	boolean a = true;
	boolean b = false;
	boolean result = a || b; // true
	```
3. `!` : Logical NOT - reverse the result/expression/value
	```java
	boolean a = true;
	boolean b = false;
	boolean result = !(a && b); // true
	``` 
	
---

#### Ternary

short-hand version of `if-else` statement. It has 3 operands thats why it got it's name "ternary".

`condition ? if true : if false`

```java
int a = 12;
int b = 10;
int result = a < 13 ? a : b; // a
// or
int result = a < 12 ? a : b; // b
```

---

#### Bitwise
use to perform operations on individual bits of a number/s and can be used on any of the integer types.


| Bit 1 | Bit 2 | AND | OR | XOR |
| --- | --- | --- | --- | --- |
| `0` | `1` | `0` | `1` | `1` |
| `0` | `0` | `0` | `0` | `0` |
| `1` | `1` | `1` | `1` | `0` |
| `1` | `0` | `0` | `1` | `1` |

1. `&` : Bitwise AND
	```java
	int a = 12;
	int b = 13;
	int result = a & b; // 12
	
	/* Explaination
	a in binary form - 1100
	b in binary form - 1101
					--------
			result	   1100
	*/
	```
	
2. `|` : Bitwise OR 
	```java
	int a = 12;
	int b = 13;
	int result = a | b; // 13
	
	/* Explaination
	a in binary form - 1100
	b in binary form - 1101
					--------
			result	   1101
	*/
	```
3. `^` : Bitwise XOR
	```java
	int a = 12;
	int b = 13;
	int result = a ^ b; // 1
	
	/* Explaination
	a in binary form - 1100
	b in binary form - 1101
					--------
			result	   0001
	*/
	```
4. `~` : Bitwise Complement
	It reverse bits of a number.
	```java
	int a = 5;
	int result = ~a; // -6
	
	/* Explaination
	First reverse the bits
	a = 5 = 0101 (starting bit sign means 
	0 = positive and 1 = negative)
	0101 => 1010
	here result's starting bit is 
	1 means number is negative, 
	
	In java negative numbers are 
	represented in 2's complement form.
	so this result is 2's complemented.
	
	To get back the original negative number
	we have to apply 2's complement the result except starting bit
	means only 010
	
	so after conversion answer will be 110 and it decimal value is 6
	also we know number is a negative number
	
	so the final answer is -6.
	
	*/
	```
	
	
#### Shift Operator
Syntax - 
```java
value/expression shift_operator number.
```
1. `<<` : Signed Left Shift
	shift the bits to left and rightmost shifted bits will be filled with `0`.
2. `>>` : Signed Right Shift
	shifts bits to the right and shifted bits are filled with sign bit of the original number.
	Steps:- 
	- Represent number in binary form (positive number is in simple binary form and negative number will be in 2's complement form).
	- Shift bits accordingly
	- The leftmost bits will be filled with sign bit.
	- Again 2's complement it except leftmost bit.

	example (in case of negative number)
	- `-10 = 10110`
	- `01011` (suppose 1 bit has be shifted)
	- `11011`
	- 2's complement of `1011` (except leftmost bit)
	- the result will be `0101` and it will negative because sign bit is `1`.
	- Decimal of the `0101` is `5` and result will be `-5`.


3. `>>>` : Unsigned right shift
	shifts the bits to the right and leftmost shifted bits will be filled witn `0`.
