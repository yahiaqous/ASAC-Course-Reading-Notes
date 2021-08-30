# Django CRUD and Forms

Forms are a flexible mechanism for collecting user input because there are suitable widgets for entering many different types of data.

An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server.

The submit input will be displayed as a button (by default) that can be pressed by the user to upload the data in all the other input elements in the form to the server.

The form attributes define the HTTP method used to send the data and the destination of the data on the server (action):

- action: The resource/URL where data is to be sent for processing when the form is submitted. If this is not set (or set to an empty string), then the form will be submitted back to the current page URL.

- method: The HTTP method used to send the data: post or get.

- The POST method should always be used if the data is going to result in a change to the server's database because this can be made more resistant to cross-site forgery request attacks.

- The GET method should only be used for forms that don't change user data.

&nbsp;

![form_handling-standard](../Pictures/form_handling-standard.png)

The main things that Django's form handling does are:

- Display the default form the first time it is requested by the user.

  - The form may contain blank fields (e.g. if you're creating a new record), or it may be pre-populated with initial values (e.g. if you are changing a record, or have useful default initial values).

  - The form is referred to as unbound at this point, because it isn't associated with any user-entered data (though it may have initial values).

- Receive data from a submit request and bind it to the form.

  - Binding data to the form means that the user-entered data and any errors are available when we need to redisplay the form.

- Clean and validate the data.

  - Cleaning the data performs sanitization of the input (e.g. removing invalid characters that might be used to send malicious content to the server) and converts them into consistent Python types.

  - Validation checks that the values are appropriate for the field (e.g. are in the right date range, aren't too short or too long, etc.)

- If any data is invalid, re-display the form, this time with any user populated values and error messages for the problem fields.

- If all data is valid, perform required actions (e.g. save the data, send an email, return the result of a search, upload a file, etc.)

- Once all actions are complete, redirect the user to another page.

How to import forms from djang?

        from django import forms

        class Form(forms.Form):
        name = forms.DateField(help_text="Data")
