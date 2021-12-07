# Forms

An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server.
Forms are a flexible mechanism for collecting user input because there are suitable widgets for entering many different types of data,
including text boxes, checkboxes, radio buttons, date pickers and so on. Forms are also a relatively 
secure way of sharing data with the server, as they allow us to send data in POST requests with cross-site request forgery protection.

Building a form
```
<form action="/your-name/" method="post">
    <label for="your_name">Your name: </label>
    <input id="your_name" type="text" name="your_name" value="{{ current_name }}">
    <input type="submit" value="OK">
</form>
```

## Declaring a Form
The declaration syntax for a Form is very similar to that for declaring a Model, and shares the same field types (and some similar parameters). 
  
  The Form class
  ```
  from django import forms

class NameForm(forms.Form):
    your_name = forms.CharField(label='Your name', max_length=100)
  ```
### Form fields
There are many other types of form fields, which you will largely recognize from their similarity to the equivalent model field classes: BooleanField, CharField, ChoiceField, TypedChoiceField, DateField, DateTimeField, DecimalField, DurationField, EmailField, FileField, etc 


### The view
Form data sent back to a Django website is processed by a view, generally the same view which published the form. This allows us to reuse some of the same logic.
