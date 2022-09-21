# Readings: Passing Functions as Props

## React Docs - lists and keys

map() function to take an array 

transforming arrays into lists of elements is nearly identical

use {} to build collection of elements 

render lists inside a component

A “key” is a special string attribute you need to include when creating lists of elements

Keys help React identify which items have changed, are added, or are removed

Keys should be given to the elements inside the array to give the elements a stable identity

The best way to pick a key is to use a string that uniquely identifies a list item among its siblings

Most often you would use IDs from your data as key

index as key last resort, don't use if order of items change in new array 

keep first compoent when extracting a key

keys unique among child components; different array different keys  

(reference: https://reactjs.org/docs/lists-and-keys.html )
## Questions 

1. What does .map() return?

a new array taht was acted upon 

2. If I want to loop through an array and display each value in JSX, how do I do that in React?

.map()

3. Each list item needs a unique ____.

key 

4. What is the purpose of a key?

Keys help React identify which items have changed, are added, or are removed

## The Spread Operator

a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments

rest parameters is also ... 

spreads can: 
Copying an array
Concatenating or combining arrays
Using Math functions
Using an array as arguments
Adding an item to a list
Adding to state in React
Combining objects
Converting NodeList to an array

Copying an array: convenient way to copy an array or combine arrays, and it can even add new items

Concatenating arrays combining two arrays into one 

(reference: https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab )

## Questions

1. What is the spread operator?

a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments; ...

2. List 4 things that the spread operator can do.

Copying an array
Concatenating or combining arrays
Using Math functions
Using an array as arguments

3. Give an example of using the spread operator to combine two arrays.

const hello = {hello: "😋😛😜🤪😝"}
const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}

const helloWorld = {...hello,...world}

4. Give an example of using the spread operator to add a new item to an array.

const fruits = ['🍏','🍊','🍌','🍉','🍍']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
fruits[0] = '🍑'
console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍

5. Give an example of using the spread operator to combine two objects into one.

const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩
## How to Pass Functions Between Components

state extist in a higher component affected by a state in a lower component is key 

(reference: https://www.youtube.com/watch?v=c05OL7XbwXU )

## Questions 

1. In the video, what is the first step that the developer does to pass functions between components?

creates incremental function in parent state, constructor function 

2. In your own words, what does the increment function do?

add value to corresponding object to a desired state by looping array with map

3. How can you pass a method from a parent component into a child component?

having a for loop with an increment function affecting a desired object; high setstate, conditional rendering

4. How does the child component invoke a method that was passed to it from a parent component?

go to child component and change local state, pass prop increment in return; this.props.increment

## Things I want to Know more about 
- button usage and I liked the updated span use
- besides increment what are some other examples for event handlers and listeners to be called 