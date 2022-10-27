# Reading Class 03

## Java OO Tutorial (only the Object and Class ones)

all have state and behavior

data encapsulation:

Hiding internal state and requiring all interaction to be performed through an object's methods

methods:

functions in some programming language

Modularity: The source code for an object can be written and maintained independently of the source code for other objects. Once created, an object can be easily passed around inside the system.

Information-hiding: By interacting only with an object's methods, the details of its internal implementation remain hidden from the outside world.

Code re-use: If an object already exists (perhaps written by another software developer), you can use that object in your program. This allows specialists to implement/test/debug complex, task-specific objects, which you can then trust to run in your own code.

Pluggability and debugging ease: If a particular object turns out to be problematic, you can simply remove it from your application and plug in a different object as its replacement. This is analogous to fixing mechanical problems in the real world. If a bolt breaks, you replace it, not the entire machine.

(reference: https://docs.oracle.com/javase/tutorial/java/concepts/object.html)

## Java Classes (do NOT do the Nested Classes section)

class declaration:

class MyClass {
    // field, constructor, and 
    // method declarations
}

class body:

the area between the braces

components of a class:

Modifiers such as public, private, and a number of others that you will encounter later. (However, note that the private modifier can only be applied to Nested Classes.)

The class name, with the initial letter capitalized by convention.
The name of the class's parent (superclass), if any, preceded by the keyword extends. A class can only extend (subclass) one parent.

A comma-separated list of interfaces implemented by the class, if any, preceded by the keyword implements. A class can implement more than one interface.

The class body, surrounded by braces, {}.

Variables Names:

the first letter of a class name should be capitalized, and

the first (or only) word in a method name should be a verb.

All variables must have a type

(reference: https://docs.oracle.com/javase/tutorial/java/javaOO/classes.html)

## Binary, Decimal and Hexadecimal Numbers

The Decimal Number System is also called "Base 10", because it is based on the number 10, with these 10 symbols:

0, 1, 2, 3, 4, 5, 6, 7, 8 and 9

there is no symbol for "ten"

10" is actually two symbols put together, a "1" and a "0

Count up until just before the "Base Number", then start at 0 again, but first you add 1 to the number on your left.

Decimal:	0	1	2	3	4	5	6	7	8	9	10	11	12	13	14	15

Hexadecimal:	0	1	2	3	4	5	6	7	8	9	A	B	C	D	E	F


(reference: https://www.mathsisfun.com/binary-decimal-hexadecimal.html)
