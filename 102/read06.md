## Introduction to CSS

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




## Colors in CSS

There are many ways to specify colors in CSS:

* ### **Color names** (common names) "***color: Cyan***"
* ### **HEX codes** (six-digit codes) "***color: #ffffff***"
* ### **RGB values** (red, green and blue) "***color: rgb(10,30,50)***"
* ### **HSL values** (hue, saturation and lightness) "***color: hsl(0,100%,100%)***"
