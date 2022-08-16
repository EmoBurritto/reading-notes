# Readings: State and Props

React lets you define components as classes or functions- lifecycle events 

The three phases of the component lifecycle:

Mounting- an instance of a component is being created and inserted into the DOM; Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount

Updating- Anytime a component is updated or state changes then it is rerendered; static getDerivedStateFromProps, shouldComponentUpdate, render,
getSnapshotBeforeUpdate, componentDidUpdate, UNSAFE_componentWillUpdate, UNSAFE_componentWillReceiveProps

Unmounting- component is being removed from the DOM; componentWillUnmount

constructor for a React component is called before it is mounted.If the component is a subclass you should call super(props), or the props will be undefined. constructors can be used to assign state using this.state or to bind event handle methods to an instance

static getDerivedStateFromProps() - exists for rare cases where the state relies on changes in props over time

render() - only required method in a class component

componentDidMount() - invoked immediately after a component is mounted

getSnapshotBeforeUpdate() - rarely used method that allows you to capture a picture of the DOM to check it before actually changing anything on the DOM

componentDidUpdate() - useful for performing network requests after a change has occurred

componentWillUnmount() - allows you to clean up the DOM and netwrok requests/ subscriptions

(refernce: https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

## React lifecycle

## Questions 

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

render

2. What is the very first thing to happen in the lifecycle of React?

mounting

3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

constructor
render
componentDidMount
React Updates
componentWillUnmount

4. What does componentDidMount do?

it applied components and subclasses on the app 

## React State Vs Props

react - abiltity to manage rendered data and rerender data when changes are made 

2 main ways of data:

props 

state 

props used over state 

props- arguements to a function 

create a component pass to a prop to render 

counter application- pass inital count 

intialize cokmpoent to, props 

count is 0 

store content on props 

component is like header 

props into components, outside 

state inside component, current counter 

props holds intital counter 

state increase and decrease counter 

props updated outside component 

change state, rerender app within that section 

props simple like information

state stores counter; hard information 

state are good for forms


(refernce: https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)
## Questions

1. What types of things can you pass in the props?

intial counter

2. What is the big difference between props and state?

props can be affected outside app, to change state, rerender app entirely 

3. When do we re-render our application?

when state is changed; counter goes up or down  

4. What are some examples of things that we could store in state?

forms 

## Things I want to Know more about 
- when to use UNSAFE lifecycle events in real situations 
- what's a counter 