# Forms in HTML

Forms enable users to search and perform other functions online


### Form Controls Types
* **Adding Text:** Text input (single-line), Password input, Text area (multi-line)
* **Making Choices:** Radio buttons, Checkboxes, Drop-down boxes
* **Submitting Forms:** Submit buttons, Image buttons
* **Uploading Files**

Every ***< form >*** element requires an **action attribute**, its value is the URL for the page on the server that will receive the information in the form when it is submitted


### Sending Forms Methods

1- **Get method**, where the values from the form are added to the end of the URL specified in the action attribute. It is ideal for:
* Short forms (such as search boxes)
* When just retrieving data from the webserver (not sending information that should be added to or deleted from a database)

2- **Post method**, where the values are sent in what is known as HTTP headers. As a general rule, the post method used if the form:
* Allows users to upload a file
* Is very long
* Contains sensitive data (e.g. passwords)
* Adds information to, or deletes information from, a database

If the method attribute is not used, the form data will be sent using the **get method**


The ***< input >***  element is used to create several different form controls. The value of the type attribute determines what kind of input they will be creating.


| **Value of the type attribute** |                                   **Function**                                   |
|---------------------------------|----------------------------------------------------------------------------------|
| type="**text**"                 | Creates a single-line text input                                                 |
| type="**password**"             | Creates a text box single-line text input and the characters are blocked out     |
| type="**radio**"                | Allow users to pick just one of a number of options                              |
| type="**checkbox**"             | Allow users to select (and unselect) one or more options in answer to a question |
| type="**file**"                 | Creates a box that looks like a text input followed by a browse button           |
| type="**submit**"               | To send a form to the server                                                     |
| type="**image**"                | To use an image for the submit button                                            |
| type="**date**"                 | Ask the user for a date                                                          |
| type="**email**"                | Ask a user for an email address                                                  |
| type="**url**"                  | Ask a user for a web page address                                                |
| type="**search**"               | Creates a single-line text box for search queries                                |

 


The ***< textarea >*** element is used to create a mutli-line text input


### Drop Down List Box
The ***< select >*** element is used to create a drop-down list box that allows users to select one option from a drop-down list. It contains two or more ***< option >*** elements that used to specify the options that the user can select from

