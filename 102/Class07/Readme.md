# Control flow

**Control flow** -  means that when you read a script, you must not only read from start to finish but also look at program structure and *how it affects order of execution*.

The *control flow* is the order in which the computer executes statements in a script.


"if else" is a conditional structure , so that different code executes depending on whether something is complete or not:
for example , if a required text field was left empty.

>if (isEmpty(field)) {
  promptUser();
} else {
  submitForm();
}


## Javascript Functions


A *JavaScript function*is a block of code designed to perform a particular task it is  executed when "something" invokes it (calls it).


A *JavaScript* function  starts with a function keyword, followed by a name, and then  by parentheses ().

Functions can contain letters, digits, underscores, and dollar signs (**same rules as variables**).

The parentheses may include parameter names separated by commas:
(parameter1, parameter2, ...)

The code to be executed, by the function, has to be placed inside curly brackets: {}

**examples**


function name (parameter1, parameter2, parameter3) {
  // code to be executed
}

Functions often compute a return value. 
The return value is "returned" back to the "user".


*Example*

let x = myFunction(4, 3);   // Function is called, return value will end up in x

function myFunction(a, b) {
  return a * b;             // Function returns the product of a and b
}


**Functions** can be used the same way as you use variables.

## Javascript Operators

There are different types of JavaScript operators:

1.Arithmetic Operators
2.Assignment Operators
3.Comparison Operators
4.Logical Operators
5.Conditional Operators
6.Type Operators

*Arithmetic Operators* are used to perform arithmetic on numbers:

+	Addition
-	Subtraction
*	Multiplication
**	Exponentiation (ES2016)
/	Division
%	Modulus (Division Remainder)
++	Increment
--	Decrement

*Comparsion Operators*

==	equal to
===	equal value and equal type
!=	not equal
!==	not equal value or not equal type
>	greater than
<	less than
>=	greater than or equal to
<=	less than or equal to
?	ternary operator


*Logical Operators*

&&	logical and
||	logical or
!	logical not


*Type Operators*

typeof	Returns the type of a variable
instanceof	Returns true if an object is an instance of an object type

*Bitwise Operators*

**Bit operators** work on 32 bits numbers.

Any numeric operand in the operation is converted into a 32 bit number.
 The result is converted back to a JavaScript number.


&	AND	5 & 1	0101 & 0001	0001	 1

|	OR	5 | 1	0101 | 0001	0101	 5

~	NOT	~ 5	 ~0101	1010	 10

^	XOR	5 ^ 1	0101 ^ 0001	0100	 4

<<	left shift	5 << 1	0101 << 1	1010	 10

>>	right shift	5 >> 1	0101 >> 1	0010	  2

>>>	unsigned right shift	5 >>> 1	0101 >>> 1	
0010	  2


**The examples above uses 4 bits unsigned examples.**  **But JavaScript uses 32-bit signed numbers.** **Because of this, in JavaScript, ~ 5 will not return 10.** **It will return -6.**
**~00000000000000000000000000000101 will return 11111111111111111111111111111010**