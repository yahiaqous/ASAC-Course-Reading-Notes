# Testing and Modules

## In Tests We Trust — TDD with Python

**Unit tests** are some pieces of code to exercise the input, the output, and the behavior of the code

**_Test-Driven Development(TDD) is a strategy to think_**

It is important to care about the files' structure,a convention widely used is the **AAA: Arrange, Act and Assert**

**Arrange**: organize the data needed to execute that piece of code (input)

**Act**: execute the code being tested (exercise the behavior)

**Assert**: after executing the code, check if the result (output) is the same as expected

**TDD: the cycle** is made by three steps:

1. Write a unit test and make it fail
2. Write the feature and make the test pass
3. Refactor the code — the first version doesn’t need to be the beautiful one

![TDDTest](Pictures/TDDTest.JPG)

&nbsp;

## If name equals main

What does the if **** name **** == “**** main ****”: do?

If the python interpreter is running module (the source file) as the main program, it sets the special **** name **** variable to have a value “**** main ****”.
If this file is being imported from another module, **** name **** will be set to the module’s name

&nbsp;

## Recursion

**Recursion**: The process in which a function calls itself directly or indirectly, and the corresponding function is called a recursive function

In the recursive program, the solution to the base case is provided and the solution of the bigger problem is expressed in terms of smaller problems.

**Direct recursion**: if the function calls the same function
**Indirect recursion**: if the function calls another function

&nbsp;

## Python Lists

### **List Methods:**

- **list.append(elem)**: adds a single element to the end of the list

- **list.insert(index, elem)**: inserts the element at the given index, shifting elements to the right

- **list.extend(list2)**: adds the elements in list2 to the end of the list. Using + or += on a list is similar to using extend()

- **list.index(elem)**: searches for the given element from the start of the list and returns its index

- **list.remove(elem)** searches for the first instance of the given element and removes it

- **list.sort()**: sorts the list in place (does not return it)

- **list.reverse()**: reverses the list in place (does not return it)

- **list.pop(index)**: removes and returns the element at the given index.(the opposite of append()).

&nbsp;

## Python Strings

A string literal can span multiple lines, but there must be a backslash \ at the end of each line to escape the newline.

String literals inside triple quotes, """ or ''', can span multiple lines of text.

### **String Methods:**

- **s.lower(), s.upper()**: returns the lowercase or uppercase version of the string

- **s.strip()**: returns a string with whitespace removed from the start and end

- **s.isalpha()/s.isdigit()/s.isspace()...**: tests if all the string chars are in the various character classes

- **s.startswith('other'), s.endswith('other')**: tests if the string starts or ends with the given other string

- **s.find('other')**: searches for the given other string (not a regular expression) within s, and returns the first index where it begins or -1 if not found

- **s.replace('old', 'new')**: returns a string where all occurrences of 'old' have been replaced by 'new'

- **s.split('delim')**: returns a list of substrings separated by the given delimiter. The delimiter is not a regular expression, it's just text. 'aaa,bbb,ccc'.split(',') -> ['aaa', 'bbb', 'ccc']. As a convenient special case s.split() (with no arguments) splits on all whitespace chars.

- **s.join(list)**: opposite of split(), joins the elements in the given list together using the string as the delimiter. e.g. '---'.join(['aaa', 'bbb', 'ccc']) -> aaa---bbb---ccc

&nbsp;

## Python Modules and Packages

**Modular programming** refers to the process of breaking a large, unwieldy programming task into separate, smaller, more manageable subtasks or modules.

Advantages of modularizing code in a large application:

- **Simplicity**
- **Maintainability**
- **Reusability**
- **Scoping**
