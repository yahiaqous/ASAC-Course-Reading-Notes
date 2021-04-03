# Objects in JavaScript


In an object, variables and functions take on new names:
* If a variable is part of an object, it is called **property**, which tells us about the object
* If a function is part of an object, it is called **method**, which represents tasks that are associated with the object

properties and methods have a name and a value called **keys**. An object cannot have two keys with the same name

### Creating an object
**Literal notation** is the easiest and most popular way to create objects, where the object is the curly braces and their contents and stored in a variable. Each key separated from its value using a *colon (:)*, and each property and method separated with a *comma (,)*

### Accessing an object
Properties and methods of an object can be accessed using *dot notation (.)* after the object name then followed its name. Properties can also be accessed using *square brackets []*



# Document Object Model (DOM)

**The Document Object Model (DOM)** specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window

As a browser loads a web page, it creates a model of that page called a **DOM tree**, and it is stored in the browser's memory.

DOM tree consists of four main types of nodes:
* **The Document Node** the starting point for all visits to the DOM tree
* **Element Nodes** its attributes and text nodes can be accessed through it
* **Attribute Nodes** part of the element that carries them, not children
* **Text Nodes** cannot have children and are always a new branches of the DOM tree

![Dom Tree](Pictures/DOM Tree.JPG)

Each node is an object with methods and properties.

### Accessing Eements

Methods that return a single element node:
* ***getElementByld ('id')***
* ***querySelector ('css selector')***

Methods that return one or more elements:
* ***getElementsByClassName ('class')***
* ***getElementsByTagName ('tagName')***
* ***querySelectorAll ('css selector')***