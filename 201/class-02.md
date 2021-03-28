# Text in HTML

**Structural Markup:** The text elements that used to describe both headings and paragraphs.

|     **Element**      |            **Tag**            |                   **Function**                    |
|----------------------|-------------------------------|---------------------------------------------------|
| **Headings**         | ***< h1 > < h2 > .. < h6 >*** | Used for main headings                            |
| **Paragraphs**       |         ***< p >***           | Create a paragraph                                |
| **Bold**             |         ***< b >***           | Make characters appear bold                       |
| **Italic**           |         ***< i >***           | Make characters appear italic                     |
| **Superscript**      |        ***< sup >***          | Make characters appear superscript                |
| **Subscript**        |        ***< sub >***          | Make characters appear subscript                  |
| **Line Breaks**      |       ***< br / >***          | Add a line break inside the middle of a paragraph |
| **Horizontal Rules** |       ***< hr / >***          | Create a break between themes                     |


**Semantic Markup:** The text elements that are not intended to affect the structure of web pages, but do add extra information to the pages

|    **Element**     |        **Tag**       |                                              **Function**                                                |
|--------------------|----------------------|----------------------------------------------------------------------------------------------------------|
| **Strong**         |   ***< strong >***   | Indicate that its content has strong importance, and displayed boldly in the browser                     |
| **Emphasis**       |     ***< em >***     | Indicates that its content subtly changes the meaning of a sentence, and displayed italic in the browser |
| **Quotations**     | ***< blockquote >*** | For longer quotes                                                                                        |
|                    |     ***< q >***      | For shorter quotes                                                                                       |
| **Abbreviations**  |   ***< abbr >***     | Specify the full term when a title attribute on the opening tag used                                     |
| **Citations**      |   ***< cite >***     | Indicate where the citation is from, and displayed italic in browser                                     |
| **Definitions**    |   ***< dfn >***      | Explain some new terminology that used first time in a document                                          |
| **Author Details** |  ***< address >***   | To contain contact details for the author of the page, and displayed italic in browser                   |
| **Delete**         |   ***< del >***      | Show content that has been inserted into a document                                                      |
| **Insert**         |   ***< ins >***      | Show text that has been deleted from a document                                                          |
| **Strikethrough**  |    ***< s >***       | Indicate that something that is no longer accurate or relevant but should not be deleted                 |


# Introducing CSS

*CSS allows creating rules that specify how the content of an element should appear*

### **Block & Inline** elements
* **Block-level elements** look like they start on a new line.
* **Inline elements** flow within the text and do not start on a new line.


### **CSS rule parts**
* **Selectors** indicate which element the rule applies to.

* **Declarations** indicate how the elements referred to in the selector should be styled, and made up of two parts:
1- Properties indicate the aspects of the element you want to change.
2- Values specify the settings you want to use for the chosen properties. 


### **Selector types**
* **Universal Selector** Applies to all elements in the document (*)
* **Type Selector** Matches element names (***elementName***)
* **Class Selector** Matches an element whose class attribute has a value that matches the one specified (***.className*** or ***p.className***)
* **Id Selector** Matches an element whose id attribute has a value that matches the one specified (***#idName***)
* **ChiLd Selector** Matches an element that is a direct child of another (***elementName>elementsName***)
* **Descendant Selector** Matches an element that is a descendent of another specified element (***elementName elementName***)
* **Adjacent Sibling Selector** Matches an element that is the next sibling of another (***elementName+elementName***)
* **General Sibling Selector** Matches an element that is a sibling of another (***elementName~elementName***)


### **Internal CSS**
by placing them inside a < style > element. (***< style type="text/css" > code < /style>***)

### **External CSS**
The *<link>* element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. It should use three attributes:
* **href** specify the path to the CSS file.
* **type** specify the type of document being linked to.
* **rel** specify the relationship between the HTML page and the file it is linked to.

Using external CSS have many benefits
* Allows all pages to use the same style rules.
* Keeps the content separate from how the page looks.
* Flexibility to change the styles used across all pages by altering just one file.
* Once the user has downloaded the CSS stylesheet, the rest of the site will load faster.



# JavaScript Instructions

**Comments** used in JavaScript to explain what the code does, and can be written in two ways:
* /* Multi-Line Comments */
* // Single-Line Comments

**Variables** (***var***): The containers for storing data values

### **Data types**
* **Numeric** for numbers
* **String** for letters and characters
* **Boolean** for true or false

Declaring variables and assigning them values can be written in different ways:
* Declaring variables and assigning values in the same statement.
* Declaring variables on the same line, then assigning values to each.
* Declaring some variables on the same line, then declaring others and assigning a value on the next line.

Naming variables rules:
* The name must begin with a letter, dollar sign ($), or an underscore (_). It must not start with a number.
* The name can contain letters, numbers, dollar signs ($), or an underscore (_). A dash(-) or a period (.) in a variable name must not be used.
* Keywords or reserved words cannot be used.
* The capital letter differs from the lowercase letter.
* Variable name should describe the kind of information that the variable stores
* "*Camel Case*" is a recommended way to write variables containing more than one word

**Array:** A special type of variable that does not just store one value; it stores a list of values.


### Types of expressions

1- Expressions that just assign a value to a variable

    *var name = 'yahia'*

2- Expressions that use two or more values to return a single value

    *var total = 1500-600*

**Operators:** Expressions used to allow programmers to create a single value from one or more values.

### Types of Operators

* **Assignment Operators** (Assign a value to a variable)
* **Arithmetic Operators** (Perform basic math)
* **Comparison Operators** (Compare two values and return true or fa1se)
* **Logical Operators** (Combine expressions and return true or fa1se)
* **String Operators** (Combine two strings)


# Decisions

### Components of decision:
1- Condition evaluation
2- Conditional statement

### Comparison Operators 

*Used to evaluate a situation by comparing one value to another and the result will be a **Boolean** (True/False).*


|    **Comparison Operator**      |                             **Task**                                   |
|---------------------------------|------------------------------------------------------------------------|
| **Equal to ==**                 | Compare two values to see if they have the same value                  |
|                                 |                                                                        |
| **Strict Equal to ===**         | Compare two values to see if they have the same value and datatype     |
|                                 |                                                                        |
| **Not Equal to !=**             | Compare two values to see if they are not the same                     |
|                                 |                                                                        |
| **Strict Not Equal to !==**     | Compare two values to see if they are not the same and datatype        |
|                                 |                                                                        |
| **Greater than >**              | Check if the left number is greater than to the right number           |
|                                 |                                                                        |
| **Greater than or Equal to >=** | Check if the left number is greater than or equal the right number     |
|                                 |                                                                        |
| **Less than <**                 | Check if the left number is less than to the right number              |
|                                 |                                                                        |
| **Less than or Equal to <=**    | Check if the left number is less than or equal the right number        |
|                                 |                                                                        |




### Logical Operators

*Used to compare the results of more than one comparison operator.*


|    **Logical Operator**      |                       **Task**                          |
|------------------------------|---------------------------------------------------------|
| **Logical And &&**           | Tests if both expressions evaluate to true              |
|                              |                                                         |
| **Logical Or**               | Tests if one of both expressions evaluates to true      |
|                              |                                                         |
| **Logical Not !**            | Inverts the Boolean value                               |
|                              |                                                         |


The "**if statement**" check a condition, if it evaluates to **true**, any statements in the subsequent code block are excuted.

The "**if...else statement**"check a condition.
If it evaluates to **true**, the first code block is excuted.
If it evaluates to **false**, the second code block is run instead.

