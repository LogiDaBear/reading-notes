# State and Props

## React lifecyle
1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
The render
2. What is the very first thing to happen in the lifecycle of React?
constructor
3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
Constructor, render, react updates, componentDidMount, componentWillUnmount
4. What does componentDidMount do?
This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions.


## React State vs Props
1. What types of things can you pass in the props?
Objects, arrays, and functions
2. What is the big difference between props and state?
Props:                                                        State:
The Data is passed from one component to another.            	The Data is passed within the component only.
It is Immutable (cannot be modified).                        	It is Mutable ( can be modified).
Props can be used with state and functional components.     	State can be used only with the state components/class component (Before 16.0).
Props are read-only.                                        	State is both read and write.
3. When do we re-render our application?
When React needs to update the app with some new data
4. What are some examples of things that we could store in state?
The current best practice is to use local state to handle the state of your user interface (UI) state rather than data. For example, using a controlled component to fill out a form is a perfectly valid use of local state.

Another example of UI data that you could store in local state would be the currently selected tab from a list of options.


## Things I want to know more about
React Native