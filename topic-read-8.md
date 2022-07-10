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

assignments are used within a variable declaration (i.e., with const, let, or var) or as standalone statements):

// Declares a variable x and initializes it to the result of f().
// The result of the x = f() assignment expression is discarded.
let x = f();

x = g(); // Reassigns the variable x to the result of g().

**assignment expressions like x = f() evaluate into a result value**

chaining or nesting an assignment expression, its result can itself be assigned to another variable:
let x;
const y = (x = f()); // Or equivalently: const y = x = f();
console.log(y); // Logs the return value of the assignment x = f().

console.log(x = f()); // Logs the return value directly.

// An assignment expression can be nested in any place
// where expressions are generally allowed,
// such as array literals' elements or as function calls' arguments.
console.log([ 0, x = f(), 0 ]);
console.log(f(0, x = f(), 0));

## Loops

Think of a loop as a computerized version of the game where you tell someone to take X steps in one direction, then Y steps in another. For example, the idea "Go five steps to the east" could be expressed this way as a loop:

for (let step = 0; step < 5; step++) {
  // Runs 5 times, with values of step 0 through 4.
  console.log('Walking east one step');
}

The statements for loops provided in JavaScript are:

for statement
do...while statement
while statement
labeled statement
break statement
continue statement
for...in statement
for...of statement

### for statement

*for loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop.*

A for statement looks as follows:

for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement
  
for loop executes, the following occurs:

The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
The conditionExpression expression is evaluated. If the value of conditionExpression is true, the loop statements execute. Otherwise, the for loop terminates. (If the conditionExpression expression is omitted entirely, the condition is assumed to be true.)
The statement executes. To execute multiple statements, use a block statement ({ ... }) to group those statements.
If present, the update expression incrementExpression is executed.
Control returns to Step 2.

### HTML

<form name="selectForm">
  <label for="musicTypes">Choose some music types, then click the button below:</label>
  <select id="musicTypes" name="musicTypes" multiple>
    <option selected>R&B</option>
    <option>Jazz</option>
    <option>Blues</option>
    <option>New Age</option>
    <option>Classical</option>
    <option>Opera</option>
  </select>
  <button id="btn" type="button">How many are selected?</button>
</form>

### JavaScript

*for statement declares the variable i and initializes it to 0. It checks that i is less than the number of options in the <select> element, performs the succeeding if statement, and increments i by 1 after each pass through the loop*
  
function howMany(selectObject) {
  let numberSelected = 0;
  for (let i = 0; i < selectObject.options.length; i++) {
    if (selectObject.options[i].selected) {
      numberSelected++;
    }
  }
  return numberSelected;
}

btn.addEventListener('click', () => {
  const musicTypes = document.selectForm.musicTypes;
  console.log(`You have selected ${howMany(musicTypes)} option(s).`);
});
  
### do...while statement

*do...while statement repeats until a specified condition evaluates to false.*

A do...while statement looks as follows:

do
  statement
while (condition);

do loop iterates at least once and reiterates until i is no longer less than 5:

let i = 0;
do {
  i += 1;
  console.log(i);
} while (i < 5);
                
## for...of statement 
                
for.of statement creates a loop Iterating over iterable objects (including Array, Map, Set, arguments object and so on), invoking a custom iteration hook with statements to be executed for the value of each distinct property
                
for (variable of object)
  statement
