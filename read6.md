# What is CSS?
![pic](https://www.w3docs.com/uploads/media/default/0001/05/6d07a36ebe6d55273b39440f2391f1d7e6d4092a.png)

CSS (Cascading Style Sheets) allows you to create great-looking web pages, but how does it work under the hood? This article explains what CSS is, with a simple syntax example, and also covers some key terms about the language.
### CSS syntax:

CSS is a rule-based language — you define rules specifying groups of styles that should be applied to particular elements or groups of elements on your web page. For example "I want the main heading on my page to be shown as large red text."

### CSS Modules :
As there are so many things that you could style using CSS, the language is broken down into modules. You'll see reference to these modules as you explore MDN and many of the documentation pages are organized around a particular module.

### How To Add CSS: 

Three Ways to Insert CSS
1. External CSS :With an external style sheet, you can change the look of an entire website by changing just one file!
Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section.
`````
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
`````
2. Internal CSS:
An internal style sheet may be used if one single HTML page has a unique style.The internal style is defined inside the <style> element, inside the head section.
`````
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
  `````
  
  3. Inline CSS
An inline style may be used to apply a unique style for a single element.To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.
  `````
  <!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>
`````
  
  




# CSS color Property:
  The color property specifies the color of text.
Tip: Use a background color combined with a text color that makes the text easy to read.
  `body {color: #92a8d1;}`
 ` body {color: rgb(201, 76, 76);}`
`  body {color: hsl(89, 43%, 51%);}`
