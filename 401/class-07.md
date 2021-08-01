# Python Scope & Big O Notation

## Python Scope

In programming, the scope of a name defines the area of a program in which one can unambiguously access that name, such as variables, functions, objects, and so on.

- **Global scope**: The names defined in this scope are available to the whole code.

- **Local scope**: The names defined in this scope are only available or visible to the code within the scope.

Since Python is a **dynamically typed language**, variables in Python come into existence when first assigned a value.

&nbsp;

### **Python Scope && Namespace**

Python scope determines wherein the program a name is visible.

Python scopes are implemented as dictionaries that map names to objects, these dictionaries are commonly called namespaces

&nbsp;

### **LEGB Rule for Python Scope**

The LEGB rule is a kind of **name lookup procedure**, which determines the order in which Python looks up names.

LEGB stand for **Local, Enclosing, Global, and Built-in**:

- **Local (or function) scope** is the code block or body of any Python function or lambda expression.

- **Enclosing (or nonlocal) scope** is a special scope that only exists for nested functions.

- **Global (or module) scope** is the top-most scope in a Python program, script, or module.

- **Built-in scope** is a special Python scope that’s created or loaded whenever you run a script or open an interactive session.

Modifying **global names** is generally considered bad programming practice because it can lead to code that is:

- **Difficult to debug**: Almost any statement in the program can change the value of a global name.

- **Hard to understand**: You need to be aware of all the statements that access and modify global names.

- **Impossible to reuse**: The code is dependent on global names that are specific to a concrete program.

Good programming practice recommends using **local names** rather than global names. Here are some tips:

- Write **self-contained functions** that rely on local names rather than global ones.

- Try to use **unique objects names**, no matter what scope you’re in.

- **Avoid global name modifications** throughout your programs.

- **Avoid cross-module name modifications**.

- **Use global names** as constants that don’t change during your program’s execution.

&nbsp;

### **builtins: The Built-In Scope**

The built-in scope is a special Python scope that’s implemented as a standard library module named builtins in Python 3.x

&nbsp;

### **Modifying the Behavior of a Python Scope**

Python provides two keywords that allow modifying the content of global and nonlocal names(global, nonlocal)

e.g: global counter # Declare counter as global
e.g: nonlocal var # Declare var as nonlocal

&nbsp;

### **Enclosing Scopes as Closures**

Closures are a **special use case of the enclosing** Python scope, which provides a way to retain state information between function calls

&nbsp;

## Big O Notation

**Big O Notation Computational Complexity**:

- **_O(1)_** - **Constant running time**
- **_O(logn)_** - **Logarithmec running time**
- **_O(n)_** - **Linear running time**
- **_O(n logn)_** - **Log-Linear running time**
- **_O(nk)_** - **Polynomial running time**
- **_O(cn)_** - **Exponential running time**
