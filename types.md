variable - name given to a memory location. it is the basic unit of storage in a program.

> int name

int  = type of data that can be stored in this variable.
name = given to the variable.


types - 
1. Primitive types - for storing simple values
2. Reference - for storing complex objects

| Type | Bytes( = 8 bits) | Value Range
| --- | ---| --- |
| byte | 1 | [-128 to 127] |
| short | 2 | [32,768 to 32,767 ] |
| int | 4 | [2,14,74,83,648 to 2,14,74,83,647] |
| long | 8 | [92,23,37,20,36,85,47,75,808 to 92,23,37,20,36,85,47,75,807] |
| float | 4 | [2,14,74,83,648 to 2,14,74,83,647] |


default java sees every whole number as int type
 and every decimal number as double type.
 
 to make long number more readable we can seperate digits with `_` like
 > int longNumber = 65_100;

string are immutable

string class has trim method which removes spaces from starting and ending of string.

array are reference type 

> int[] numbers = new int[5];

if we know values in the array we can initialize it by
 #### older way
 > numbers[0] = 1;
 > numbers[1] = 2;
 > ...
 
 #### newer way
 
 > int[] numbers = {1,2};

to print array

we use method name toString in Array class.

> Array.toString(_ARRAYNAME_);

but toString only works for 1d arrays.

to print multi dimensional arrays

use deepToString method in place of toString.

constants are variable which value can't be changed after initial initialization.

> final int num = 12;

`+=` is augmented assignment operator