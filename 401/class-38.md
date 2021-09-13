# React 2

## React - Conditional Rendering

In React, you can create distinct components that encapsulate the behavior you need. Then, you can render only some of them, depending on the state of your application

Conditional Rendering Methods:

- **Element Variables**

- **Inline If with Logical && Operator**

- **Inline If-Else with Conditional Operator**

- **Preventing Component from Rendering**

&nbsp;

## React - Lists & Keys

- **Rendering Multiple Components**

  We can build collections of elements and include them in JSX using curly braces {}

- **Basic List Component**

  Usually, you would render lists inside a component

- **Keys**

  Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity

- **Extracting Components with Keys**

  Keys only make sense in the context of the surrounding array

- **Keys Must Only Be Unique Among Siblings**

  Keys used within arrays should be unique among their siblings. However, they don’t need to be globally unique. We can use the same keys when we produce two different arrays

&nbsp;

## React - Forms

HTML form elements work a bit differently from other DOM elements in React because form elements naturally keep some internal state

- **Controlled Components**

  In HTML, form elements such as **_< input >_**, **_< textarea >_**, and **_< select >_** typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components and only updated with setState()

- **The textarea Tag**

  In HTML, a **_< textarea >_** element defines its text by its children. In React, a **_< textarea >_** uses a value attribute instead. This way, a form using a **_< textarea >_** can be written very similarly to a form that uses a single-line input

- **The select Tag**

  In HTML, **_< select >_** creates a drop-down list. For example, this HTML creates a drop-down list of flavors. In React, instead of using this selected attribute, uses a value attribute on the root select tag. This is more convenient in a controlled component because you only need to update it in one place

- **The file input Tag**

  In HTML, an **_< input type="file" >_** lets the user choose one or more files from their device storage to be uploaded to a server or manipulated by JavaScript via the File API. Because its value is read-only, it is an uncontrolled component in React

- **Handling Multiple Inputs**

  When you need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name

- **Controlled Input Null Value**

Specifying the value prop on a controlled component prevents the user from changing the input unless you desire so. If you’ve specified a value but the input is still editable, you may have accidentally set the value to undefined or null

&nbsp;

## React - Lifting State

There should be a single “source of truth” for any data that changes in a React application. Usually, the state is first added to the component that needs it for rendering. Then, if other components also need it, you can lift it up to their closest common ancestor. Instead of trying to sync the state between different components, you should rely on the top-down data flow

Lifting state involves writing more “boilerplate” code than two-way binding approaches, but as a benefit, it takes less work to find and isolate bugs. Since any state “lives” in some component and that component alone can change it, the surface area for bugs is greatly reduced. Additionally, you can implement any custom logic to reject or transform user input

&nbsp;

## React - Composition vs Inheritance

- **Containment**

  Some components don’t know their children ahead of time. This is especially common for components like Sidebar or Dialog that represent generic “boxes”

- **Specialization**

  Sometimes we think about components as being “special cases” of other components
