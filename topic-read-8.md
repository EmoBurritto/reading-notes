## Reflection and Discussion

## Expressions and Operators

### Operators

The different type of operators: 
Assignment operators
Comparison operators
Arithmetic operators
Bitwise operators
Logical operators
String operators
Conditional (ternary) operator
Comma operator
Unary operators
Relational operators

JavaScript has both binary and unary operators; one special ternary operator, the conditional operator

binary operator: 
operand1 operator operand2
3+4 or x*y

unary operator: 
operator operand
x++

operand operator
++x

### Assignment operators

Name	Shorthand operator	Meaning
Assignment	x = f()	x = f()
Addition assignment	x += f()	x = x + f()
Subtraction assignment	x -= f()	x = x - f()
Multiplication assignment	x *= f()	x = x * f()
Division assignment	x /= f()	x = x / f()
Remainder assignment	x %= f()	x = x % f()
Exponentiation assignment	x **= f()	x = x ** f()
Left shift assignment	x <<= f()	x = x << f()
Right shift assignment	x >>= f()	x = x >> f()
Unsigned right shift assignment	x >>>= f()	x = x >>> f()
Bitwise AND assignment	x &= f()	x = x & f()
Bitwise XOR assignment	x ^= f()	x = x ^ f()
Bitwise OR assignment	x |= f()	x = x | f()
Logical AND assignment	x &&= f()	x && (x = f())
Logical OR assignment	x ||= f()	x || (x = f())
Logical nullish assignment	x ??= f()	x ?? (x = f())

### Assigning to properties

*expression to an object*

let obj = {};

obj.x = 3;
console.log(obj.x); // Prints 3.
console.log(obj); // Prints { x: 3 }.

const key = "y";
obj[key] = 5;
console.log(obj[key]); // Prints 5.
console.log(obj); // Prints { x: 3, y: 5 }.

*expression does not evaluate to an objec*

let val = 0;

console.log(val.x = 3); // Prints 3.
console.log(val.x); // Prints undefined.
console.log(val); // Prints 0.

**error to assign values to unmodifiable properties or to properties of an expression without properties**

null or undefined

### Destructing 

*expression that makes it possible to extract data from arrays or objects using a syntax that mirrors the construction of array and object literals*

var foo = ['one', 'two', 'three'];

// without destructuring
var one   = foo[0];
var two   = foo[1];
var three = foo[2];

// with destructuring
var [one, two, three] = foo;

### Evaluating and nesting 

*assignments are used within a variable declaration (i.e., with const, let, or var) or as standalone statements)*

// Declares a variable x and initializes it to the result of f().
// The result of the x = f() assignment expression is discarded.
let x = f();

x = g(); // Reassigns the variable x to the result of g().

**assignment expressions like x = f() evaluate into a result value**

## Loops
