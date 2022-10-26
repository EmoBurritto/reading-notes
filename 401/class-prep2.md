# Prep: Data Structures and Algorithms

## Basic Recursion

recursion is in all algorithms 

broken down into base case and recursive case 

pseudo high level description of problem you are trying to solve in plain english 

recursion is when function calls itself  

recursion is used for readability not performance 

easy to make infinite loop when making a recursion 

when infinite loop occurs, ctrl c to kill loop 

base case- function does not call itself to break loop 

recursive case- function calls itself 

(reference: https://www.youtube.com/watch?v=vPEJSJMg4jY)

## Data Structures in 15 Minutes

without data structures can't solve algorithms

without algorithms can't pass interview

data structure 

grouped data items is compound data 

stored compound data is data structure 

Big O notation, grades behavior of data structure abilities on compound data

5 most important data structures: 

Linked Lists

- atomic unit is a node

- node contains value and pointer 

- value is like number object and pointer directs to next chained value 

- head is the first value, first pointer 

- tail is the last value with no pointer 

- good at adding, deleting new nodes 

- bad at retrieving, searching nodes 

- nodes are only away of node next to it, no index 

Array

- most common in all programming languages 

- continuous block of cells in computer memory 

- keep track memory location, index

- good at retrieving items 

- bad at adding items, overflow array, memory

- high level languages like JS and Python take care of problem 

- low level languages means declare size of array in advance 

Hash Table

- like object in JS or dictionary in Python 

- key runs through hashing function returns memory location 

- memory locations can be anywhere 

- two keys can hash into same memory location, collision 

Stack and Que 

- stack, last in first out data structure 

- push to add

- pop to remove

- order is kept by call stack 

- call stack important for DFS, algorithm depth for search

- Que first in first out 

- enqueue add 

- dequeue remove

- important fro BFS, algorithm breadth for search

- both have sufficient add remove 

- limited cases 

Graphs and Trees 

- entire CS dedicated to graph theory 

- graphs similar to linked lists 

- nodes but with edges for pointers 

- edges can have weight, numbers, between nodes and edges

- more complex hierarchal graph is a tree 

- parent child relationship 

- binary search tree 

- really specific rules to allow for easier searching 

- nodes only have two children 

- left < node

- right > node

-unbalance tree by adding too many elements, no longer efficient 

(reference: https://www.youtube.com/watch?v=vPEJSJMg4jY)
## Big O Explained

algorithm efficiency is Big O

equation in asking how time scales with respect to some input variables 

O(N) size of array is linear 

O(N2) two pairs, so squared, time it takes to run code 

you don't have to use N, any variable will work 

describe run time 

4 important rules 

- add up all steps in algorithm to find run time; o(a) O(b) = O(a+b)

- drop constants

- different inputs, different variables to represent them; two array is O(a*b)

- drop non dominant terms

(reference: https://www.youtube.com/watch?v=vPEJSJMg4jY)

## Why Big O

Big-O is just the name of the notation used to describe how efficient an algorithm is

not memory, break down algorithm to see run time 

allow code to run in a reasonable amount of time and take up a reasonable amount of space

algorithm and Big O go hand in hand
 
(reference: https://www.youtube.com/watch?v=vPEJSJMg4jY)

## Questions 

1. What is 1 of the more important things you should consider when deciding which data structure is best suited to solve a particular problem?

decide what benefit you want when manipulating data, adding or removing, etc; Big O notation 

2. How can we ensure that we’ll avoid an infinite recursive call stack?

have both a clear base case and recursive case 

## Things I want to know more about
- do we memorize Big O values?