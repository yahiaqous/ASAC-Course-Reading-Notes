# List Comprehensions & Python Decorators

## List Comprehensions

List comprehensions provide **a concise way to create lists**.

**_new_list = [expression(i) for i in old_list if filter(i)]_**

- **_new_list_** The new list (result).

- **_expression(i_** Expression is based on the variable used for each element in the old list.

- **_for i in old_list_**: The word for followed by the variable name to use, followed by the word in the old list.

- **_if filter(i)_**: Apply a filter with an If-statement.

**_[i for i in range(10)]_** returns **[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]**

Example:

**_string = "Hello 12345 World"_**

**_numbers = [x for x in string if x.isdigit()]_**

**_print numbers_**

> > **['1', '2', '3', '4', '5']**

- Change x.isdigit() to x.isalpha() if you don’t want any numbers.

&nbsp;

## Primer on Python Decorators

A decorator is a function that takes another function and extends the behavior of the latter function without explicitly modifying it.

**Decorators wrap a function, modifying its behavior**.

- Decorators can be **reused**.
- Decorators can decorate functions with **arguments and return values**.
- Decorators can use @functools.wraps to **look more like the decorated function**.

### **Decorating Functions With Arguments**

Normally can not decorate a function that accepts some arguments, the solution is to use \*args and \*\*kwargs in the inner wrapper function

    def do_twice(func):

        def wrapper_do_twice(*args, **kwargs):

            func(*args, **kwargs)

            func(*args, **kwargs)

        return wrapper_do_twice

### **Registering Plugins**

Decorators don’t have to wrap the function they’re decorating. They can also simply register that a function exists and return it unwrapped. This can be used, for instance, to create a light-weight plug-in architecture, The @register decorator simply stores a reference to the decorated function in the global PLUGINS dict

### **Decorating Classes**

There are two different ways to use **decorators in classes**:

- By decorate **the methods of a class**
- By decorate **the whole class**

### **Stateful Decorators**

Sometimes, it’s useful to have a decorator that can keep track of state. As a simple example, a decorator counts the number of times a function is called.
