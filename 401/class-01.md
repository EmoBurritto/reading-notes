# Readings: Java Basics

## The Java™ Tutorials

Variables: 

- object stores data(state) in fields 

4 main type of variables: 

- Instance Variables (Non-Static Fields) - values unique to each instance of a class 

- Class Variables (Static Fields) - value of a class, one of a kind, can be instantiated(creating) multiple time, still one value 

- Local Variables - method stores temporary state(value), locally scoped only  

- Parameters - always classified as variables not fields

Naming: 

- case sensitive 

- no white space 

- $ and _ permitted to start naming, HIGHLY discouraged 

- use full words, no abbreviations 

- camel case 


Java programming language is statically-typed, which means that all variables must first be declared before they can be used

int gear = 1

int = data type 

gear = field 

1 = value 

8 Primitive Data Type 

- byte default value(for fields) 0

- short default value(for fields) 0

- int default value(for fields) 0

- long default value(for fields) 0L

- float default value(for fields) 0.0f

- double default value(for fields) 0.0d

- boolean default value(for fields) false 

- char default value(for fields) 	'\u0000'

primitives are literals due to having set values 

to declare an array you need to have array type, byte[] and array name anArr

arraycopy is teh method used to copy arrays 

The length of an array is established when the array is created. After creation, its length is fixed

Operators:

postfix	
expr++ expr--

unary	
++expr --expr +expr -expr ~ !

multiplicative	
* / %

additive	
+ -

shift	
<< >> >>>

relational	
< > <= >= instanceof

equality	
== !=

bitwise AND	
&

bitwise exclusive OR	
^

bitwise inclusive OR	
|

logical AND	
&&

logical OR	
||

ternary	
? :

assignment	
= += -= *= /= %= &= ^= |= <<= >>= >>>=

Arithmetic:
+	
Additive operator (also used for String concatenation)

-	
Subtraction operator

*	
Multiplication operator

/	
Division operator

%	
Remainder operator

= can be assignment and object reference 
combine arithmetic opertors to create compound assignments x+=1 is equal to x= x+1
Unary Operator: 

require one operand 

perform various operations such as incrementing/decrementing a value by one, negating an expression, or inverting the value of a boolean

+	
Unary plus operator; indicates positive value (numbers are positive without this, however)

-	
Unary minus operator; negates an expression

++	
Increment operator; increments a value by 1

--	
Decrement operator; decrements a value by 1

!	
Logical complement operator; inverts the value of a boolean

prefix version (++result) evaluates to the incremented value, whereas the postfix version (result++) evaluates to the original value

Equality and Relational Operators:

==      equal to
!=      not equal to
>       greater than
>=      greater than or equal to
<       less than
<=      less than or equal to

use == no = when comparing two primitive values are equal

Conditional Operators

&& Conditional-AND
|| Conditional-OR

The && and || operators perform Conditional-AND and Conditional-OR operations on two boolean expressions. These operators exhibit "short-circuiting" behavior, which means that the second operand is evaluated only if needed.

?:, which can be thought of as shorthand for an if-then-else;  "If someCondition is true, assign the value of value1 to result. Otherwise, assign the value of value2 to result."

Type Comparison Operator instanceof:

The instanceof operator compares an object to a specified type. You can use it to test if an object is an instance of a class, an instance of a subclass, or an instance of a class that implements a particular interface

When using the instanceof operator, keep in mind that null is not an instance of anything

Bitwise and Bit Shift Operators:

The unary bitwise complement operator "~" inverts a bit pattern

The signed left shift operator "<<" shifts a bit pattern to the left, and the signed right shift operator ">>" shifts a bit pattern to the right.

The bitwise & operator performs a bitwise AND operation.

The bitwise ^ operator performs a bitwise exclusive OR operation.

The bitwise | operator performs a bitwise inclusive OR operation

Expressions, Statements, and Blocks:

Operators may be used in building expressions, which compute values; expressions are the core components of statements; statements may be grouped into blocks

An expression is a construct made up of variables, operators, and method invocations, which are constructed according to the syntax of the language, that evaluates to a single value

A statement forms a complete unit of execution ended by a ; 

expression statements:

- Assignment expressions

- Any use of ++ or --

- Method invocations

- Object creation expressions

A declaration statement declares a variable

Control flow statements regulate the order in which statements get executed

A block is a group of zero or more statements between balanced braces and can be used anywhere a single statement is allowed

Control Flow Statement:

usually code read PEMDAS

break up the flow of execution by employing decision making, looping, and branching, enabling your program to conditionally execute particular blocks of code

The if-then Statement:

tells program to execute a certain section of code only if a particular test evaluates to true

The if-then-else statement:

provides a secondary path of execution when an "if" clause evaluates to false

The switch Statement:

works with all objects

The body of a switch statement is known as a switch block. A statement in the switch block can be labeled with one or more case or default labels

evaluates its expression, then executes all statements that follow the matching case label

The while and do-while Statements:

continually executes a block of statements while a particular condition is true

must return a boolean value

The difference between do-while and while is that do-while evaluates its expression at the bottom of the loop instead of the to

The for Statement:

provides a compact way to iterate over a range of value


(reference: https://docs.oracle.com/javase/tutorial/java/nutsandbolts/index.html)

## Java Reddit Thread

compiling code is translating human friendly language into computer 1 and 0's to execute desired code
(reference: https://www.reddit.com/r/explainlikeimfive/comments/233dq5/eli5_what_does_it_mean_to_compile_code/)

## XKCD: Compiling 

compiling code can take some time if wrong primitive data types and other objects types used incorrectly 

(reference: https://xkcd.com/303/)

## Questions 

1. What does “strong typed” mean?

demands the declaration of every variable with a data type

(reference: https://www.google.com/search?q=what+does+strong+type+mean+in+java&rlz=1C1ONGR_enUS1012US1012&oq=what+does+strong+type+mean+in+java&aqs=chrome..69i57j0i15i22i30j0i390l4.5384j1j15&sourceid=chrome&ie=UTF-8)

2. Explain to a non-technical friend the difference in how compilation works in Java and JavaScript.

computer obtains sentence attempts to read passage 
computer gets passage breaks down by paragraph 
paragraph broken down into sentences 
sentences broken down by words
bigger syllable words, more time to read
words understood 
sentence understood 
passage understood 
passage read    

## Things I want to know more about
- need more clarification of primitive type and when to use them, do we memorize the file size like byte is 127 characters?
- instanceof is like using methods ina constructor function in REACT?
- when bitwise operators are used 