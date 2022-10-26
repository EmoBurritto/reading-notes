# Reading Class 03

## Primitives vs. Objects

Java has a two-fold type system consisting of primitives such as int, boolean and reference types such as Integer, Boolean

Every primitive type corresponds to a reference type

wrapper classes are immutable (so that their state can't change once the object is constructed) and are final (so that we can't inherit from them)

memory key factor when choosing what object to use 

impact on memory:

boolean – 1 bit
byte – 8 bits
short, char – 16 bits
int, float – 32 bits
long, double – 64 bits

single-element arrays of primitive types are almost always more expensive (except for long and double) than the corresponding reference type

primitive types may acquire values only from their domains, while the reference types might acquire a value (null) that in some sense doesn't belong to their domains

(reference: https://www.baeldung.com/java-primitives-vs-objects)

## Exceptions in Java (read the first three sections on the left: What is an Exception, The Catch or Specify Requirement, Catching and Handling Exceptions)

exceptions are to handle errors and other exceptional events

shorthand for the phrase "exceptional event"

an event, which occurs during the execution of a program, that disrupts the normal flow of the program's instructions

error occurs within a method

object is created called exception object and passed to runtime system 

creating an exception object and handing it to the runtime system is called throwing an exception

call stack to find possible solution to exception 

exception handler is found when call stack finds solution, done by starting at exception and going in reverse order to find solution 

exception handler catches the exception 

no exception handler found, app terminates 

(reference: https://docs.oracle.com/javase/tutorial/essential/exceptions/index.html)

## Using Scanner to read in a file in Java

useful for breaking down formatted input into tokens and translating individual tokens according to their data type

By default, a scanner uses white space to separate tokens

 treats all input tokens as simple String values. Scanner also supports tokens for all of the Java language's primitive types (except for char), as well as BigInteger and BigDecimal
 
(reference: https://docs.oracle.com/javase/tutorial/essential/io/scanning.html)
