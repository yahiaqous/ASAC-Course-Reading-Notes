# State and Props

## Phases of the component lifecycle:
1- **Mounting:** When an instance of a component is being created and inserted into the DOM

2- **Updating:** Anytime a component is updated or state changes then it is rerendered

3- **Unmounting:** When a component is being removed from the DOM


| **Method**                            | **Example Uses**                              |
|---------------------------------------|-----------------------------------------------|
| **render()**                          | Create and return elements                    |
| **componentDidMount()**               | DOM manipulations, network requests, ...etc   |
| **static getDerivedStateFromProps()** | Update state based on changed props           |
| **shouldComponentUpdate()**           | Compare inputs and determine if render needed |
| **getSnapshotBeforeUpdate()**         | Set/reset things before next render           |
| **componentDidUpdate()**              | DOM manipulations, network requests, ...etc   |
| **componentWillUnmount()**            | DOM manipulations, network requests, ...etc   |



### Questions
* Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
**componentDidMount**

* What is the very first thing to happen in the lifecycle of React?
**Mounting**

* Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates.
**constructor, componentDidMount, render, React Updates, componentWillUnmount**

* What does componentDidMount do?
**DOM manipulations, network requests, ...etc**


## React State Vs Props:
### Questions
* What types of things can you pass in the props?


* What is the big difference between props and state?
**Props is handled outside of the component and state is handled inside of that component**

* When do we re-render our application?
**When the data changes**

* What are some examples of things that we could store in state?
**Forms, counter**