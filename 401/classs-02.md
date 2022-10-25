# Readings: Class 02

## Java Imports 

Java Package: 

A package is simply a container that groups related types (Java classes, interfaces, enumerations, and annotations)

help to reserve the class namespace and create a maintainable code

user-defined packages:

allows to create packages as per your need

JDK comes with existing java packages 

define package name using package keyword

package packageName;

package name must be unique (like a domain name), but in reverse order of hierarchy 

(reference: https://www.programiz.com/java-programming/packages-import)

## Different types of loops in Java

looping is a feature which facilitates the execution of a set of instructions until the controlling Boolean-expression evaluates to false

types of loops: 

Simple for loop- a control structure that allows us to repeat certain operations by incrementing and evaluating a loop counter

Enhanced for-each loop

While loop- repeats a statement or a block of statements while its controlling Boolean-expression is true

Do-While loop- works just like the while loop except for the fact that the first condition evaluation happens after the first iteration of the loop

(reference: https://www.baeldung.com/java-loops)

## Java Arrays

stores a fixed-size sequential collection of elements of the same type, collection of variables 

to declare an array, you must declare a variable to reference the array, and you must specify the type of array the variable can reference

dataType[] arrayRefVar;   // preferred way.
or
dataType arrayRefVar[];  // works but not preferred way.


to create new array use : 

arrayRefVar = new dataType[arraySize];

When processing array elements, we often use either for loop or foreach loop because all of the elements in an array are of the same type and the size of the array is known

for each allows complete array to be invoked without using index variable
can pass arrays into methods

method can return an array 

Array Class:

public static int binarySearch(Object[] a, Object key)

Searches the specified array of Object ( Byte, Int , double, etc.) for the specified value using the binary search algorithm. The array must be sorted prior to making this call. This returns index of the search key, if it is contained in the list; otherwise, it returns ( – (insertion point + 1)).
	
public static boolean equals(long[] a, long[] a2)

Returns true if the two specified arrays of longs are equal to one another. Two arrays are considered equal if both arrays contain the same number of elements, and all corresponding pairs of elements in the two arrays are equal. This returns true if the two arrays are equal. Same method could be used by all other primitive data types (Byte, short, Int, etc.)

public static void fill(int[] a, int val)

Assigns the specified int value to each element of the specified array of ints. The same method could be used by all other primitive data types (Byte, short, Int, etc.)

public static void sort(Object[] a)

Sorts the specified array of objects into an ascending order, according to the natural ordering of its elements. The same method could be used by all other primitive data types ( Byte, short, Int, etc.)

(reference: https://www.tutorialspoint.com/java/java_arrays.htm)



## Questions 

1. Which loops use a loop counter?

for and for-each loop 

2. Describe 3 built-in methods for Arrays.

public static int binarySearch(Object[] a, Object key)

Searches the specified array of Object ( Byte, Int , double, etc.) for the specified value using the binary search algorithm. The array must be sorted prior to making this call. This returns index of the search key, if it is contained in the list; otherwise, it returns ( – (insertion point + 1)).
	
public static boolean equals(long[] a, long[] a2)

Returns true if the two specified arrays of longs are equal to one another. Two arrays are considered equal if both arrays contain the same number of elements, and all corresponding pairs of elements in the two arrays are equal. This returns true if the two arrays are equal. Same method could be used by all other primitive data types (Byte, short, Int, etc.)
	
public static void fill(int[] a, int val)

Assigns the specified int value to each element of the specified array of ints. The same method could be used by all other primitive data types (Byte, short, Int, etc.)

(reference: https://www.tutorialspoint.com/java/java_arrays.htm)

3. Use an analogy to explain Built-In packages. Give examples.

built in packages is like using xbox game PC and being able to play the same game cross platform on xbox or PC and being able to pick up on a saved gam from  Xbox to PC. 



## Things I want to know more about
-built in package from JDK just 4?
