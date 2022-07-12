# Readings: State and Props

## React Lifecyle

Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

- based off the [diagram](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093) in the readings, render seems like it happened first.

What is the very first thing to happen in the lifecycle of React?

- Mounting

Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

- Constructor, Render, React Updates, componentDidMount, componentWillUnmount.

What does componentDidMount do?

- it is invoked immediately after a component is mounted and loads anything using a network request or initialize the DOM.

## React State Vs Props

What types of things can you pass in the props?

- the initial component to a function, title and subtitle.

What is the big difference between props and state?

- state is handled inside of the component and props is handled outside of the component.

When do we re-render our application?

- when we change the state inside of our application it re-renders the application.

What are some examples of things that we could store in state?

- When something needs to be updated when a User makes an interaction on a website. Like a counter or a Form.

## Things I want to know more about

How to properly use state code wise. I want to see how a state can effectively affect our application.
