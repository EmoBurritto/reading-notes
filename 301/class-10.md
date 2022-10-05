# Readings: In memory storage

## Understanding the JavaScript Call Stack

The JavaScript engine (which is found in a hosting environment like the browser), is a single-threaded interpreter comprising of a heap and a single call stack. The browser provides web APIs like the DOM, AJAX, and Timers.

The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

Asynchronous JavaScript, we have a callback function, an event loop, and a task queue.

At the most basic level, a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

The key takeaways from the call stack are:
1. It is single-threaded. Meaning it can only do one thing at a time.
2. Code execution is synchronous.
3. A function invocation creates a stack frame that occupies a temporary memory.
4. It works as a LIFO — Last In, First Out data structure.

(reference: https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)
## Questions 

1. What is a ‘call’?

function invocation 

2. How many ‘calls’ can happen at once?

3. What does LIFO mean?

last in first out 

4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

function firstFunction(){
  console.log("Hello from firstFunction");
}

function secondFunction(){
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();

5. What causes a Stack Overflow?

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point

## JavaScript error messages

reference error
when using const and let, they are hoisted like var and function but there is a time between the hoisting and being declared so when you try to access them a reference error occurs, the fact that this happens to let and const is called Temporal Dead Zone (TDZ).

syntax error
occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

range error 
Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

type error 
this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

breakpoint 
the line you selected was run you will be able to see what has happened before that point and you can try and evaluate the next lines to check if everything is outputting what you are expecting

debugger 

(reference: https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)
## Questions

1. What is a ‘reference error’?

when using const and let, they are hoisted like var and function but there is a time between the hoisting and being declared so when you try to access them a reference error occurs, the fact that this happens to let and const is called Temporal Dead Zone (TDZ).

2. What is a ‘syntax error’?

occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

3. What is a ‘range error’?

Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

4. What is a ‘type error’?

this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

5. What is a breakpoint?

the line you selected was run you will be able to see what has happened before that point and you can try and evaluate the next lines to check if everything is outputting what you are expecting

6. What does the word ‘debugger’ do in your code?

breakpoints within vs code 

## Things I want to Know more about 
- proper use of debugger in vs code, don't feel comfortabel using tool yet, need a class on it 