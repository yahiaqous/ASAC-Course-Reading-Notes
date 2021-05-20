# Thinking in React


## The process of building a searchable product data table using React:
### **Step 1:** Break The UI Into A Component Hierarchy
### **Step 2:** Build A Static Version in React
### **Step 3:** Identify The Minimal (but complete) Representation Of UI State
### **Step 4:** Identify Where Your State Should Live
### **Step 5:** Add Inverse Data Flow


### Questions
* How would you break a mock into a component hierarchy?
**By drawing boxes around every component (and subcomponent) in the mock and give them all names**

* What is the single responsibility principle and how does it apply to components?
**A component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents**

* What does it mean to build a ‘static’ version of your application?
**Build a version that takes data model and renders the UI but has no interactivity**

* Once you have a static application, what do you need to add?
**Make the user interface interactive**

* What are the three questions you can ask to determine if something is state?

  * **Is it passed in from a parent via props? If so, it probably isn’t state.**

  * **Does it remain unchanged over time? If so, it probably isn’t state.**

  * **Can you compute it based on any other state or props in your component? If so, it isn’t state**

* How can you identify where state needs to live?

  * **Identify every component that renders something based on that state.**

  * **Find a common owner component (a single component above all the components that need the state in the hierarchy).**

  * **Either the common owner or another component higher up in the hierarchy should own the state.**

  * **If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.**




















