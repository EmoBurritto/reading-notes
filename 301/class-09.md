# Readings: Functional Programming

## Functional Programming Concepts

Pure functions: 
It returns the same result if given the same arguments (it is also referred as deterministic)
It does not cause any observable side effects

An impure function would receive radius as the parameter, and then calculate radius * radius * PI:

If our function reads external files, it’s not a pure function — the file’s contents can change.

Any function that relies on a random number generator cannot be pure.

Examples of observable side effects include modifying a global object or a parameter passed by reference.

Pure function benefits:
Given a parameter A → expect the function to return value B
Given a parameter C → expect the function to return value D

When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.


(reference: https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)
## Questions 

1. What is functional programming?

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 

2. What is a pure function and how do we know if something is a pure function?

It returns the same result if given the same arguments (it is also referred as deterministic)
It does not cause any observable side effects

3. What are the benefits of a pure function?

returns same parameters in a new function; no side effects or relying on external files  

4. What is immutability?

Unchanging over time or unable to be changed.

5. What is Referential transparency?

if a function consistently yields the same result for the same input; pure functions + immutable data = referential transparency
## Node JS Tutorial for Beginners #6 - Modules and require()

never put everything in APP.js

split code into logical modules 

each module has certain functionality 

called in app to be displayed 

./ is current directory

(reference: https://www.youtube.com/watch?v=xHLd36QoS4k)
## Questions

1. WWhat is a module?

an external file with certain functionality in order to make overall app dev friendly 

2. What does the word ‘require’ do?

allows modules to be used in App.js with global functions 

3. How do we bring another module into the file the we are working in?

import

4. What do we have to do to make a module available?

export

## Things I want to Know more about
- examples of when we used pure function becuase I feel like everythign we have done at this point isn't 