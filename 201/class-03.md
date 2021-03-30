# Lists in HTML

### Types of lists

|     **List Type**     |   **Tag**    |                            **Function**                                      |
|-----------------------|--------------|------------------------------------------------------------------------------|
|   **Ordered lists**   | ***< ol >*** | where each item in the list is numbered                                      |
| **Unordered lists**   | ***< ul >*** | that begin with a bullet point                                               |
| **Definition lists**  | ***< dl >*** | made up of a set of terms along with the definitions for each of those terms |


Lists can be nested inside each other



# Boxes in CSS

The most popular ways to specify the size of a box are to use **pixels**, **percentages**, or **ems**.

### Limiting Dimension: ***min-width***, ***max-width***, ***min-height***, ***max-height***
Used in order to specify the smallest/maximum size a box can be displayed at when the browser window is narrow/wide,

### Overflowing Content: ***overflow***
Used to tell the browser what to do if the content contained within a box is larger than the box itself, and can have one of two values:
* ***hidden*** hide any extra content
* ***scroll*** add a scrollbar to the box

Every box has three available properties that can be adjusted to control its appearance:
1- **Border:** The limit that separates the edge of one box from another
2- **Margin:** The space outside the edge of the border between the borders of adjacent boxes
3- **Padding:** The space between the border of a box and any content contained within it

### Border width, style, and color: 
* ***border-width*** can be in *pixels* or *thin* - *medium* - *thick*
* ***border-style*** can be *solid* - *dotted* - *dashed* - *double* - *groove* - *ridge* - *inset* - *outset* - *hidden*/*none*
* ***border-color***

### Change inline/block: ***display***
Turn an inline element into a block-level element or vice versa, and can hide an element from the page

### Hiding Boxes: ***visibility***
Hide boxes from users but it leaves a space where the element would have been

### Box Shadows: ***box-shadow***
with horizontal offset, vertical offset, blur distance, the spread of shadow, and color



# Arrays, Decisions and Loops in JavaScript

**Array:** A special type of variable that does not just store one value; it stores a list of values.

The **"if...else statement"** check a condition, then:
* If it evaluates to true, the first code block is executed.
* If it evaluates to false, the second code block is run instead.

The **"switch statement"** starts with a variable (**the switch value**), each case indicates a possible value for this variable and the code that should run if the variable matches that value, at the end of each case is the break keyword. The "**default**" option runs if none of the cases match.

### Truthy & Falsy Values
* Truthy values are treated as if they are *true*, can be treated as the number *0*
* Falsy values are treated as if they are *fa1se*, can be treated as the number *1*

*false*, *0*, and *' '* (empty string) considered equal when using **==**, but they are not equivalent when using the strict operator **===**

*NaN*, *null* and *undefined* are both falsy, they are not equal to anything other than themselves.


### Loops

*Used to check a condition, if it evaluates to true, a code block will run until the condition evaluates to false.*


|    **Loop**     |                                            **Task**                                                      |
|-----------------|----------------------------------------------------------------------------------------------------------|
| **FOR**         | The code will be running a specific number of times                                                      |
|                 |                                                                                                          |
| **WHILE**       | The code will be running as long as the condition is True                                                |
|                 |                                                                                                          |
| **DO WHILE**    | The code will run at least once even the condition is false and running as long as the condition is True |
|                 |                                                                                                          |

**For loop** is made up of three statements:

- **Initialization**: Create a variable.

- **Condition**: Made of Comparison or Logical operator statement.

- **Update**: The change that will happen every time after the loop code finish.


**While loop** is made up of a condition statement only.

