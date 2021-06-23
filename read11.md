# Links:
Links are the defining feature of the web because they allow you to move from one web page to another — enabling the very idea of browsing or surfing.

### Writing Links:

Links are created using the  `<a>`  element. Users can click on anything between the opening `<a>` tag and the closing `</a>` tag. You specify which page you want to link to using the href attribute.
![](https://www.computerhope.com/jargon/h/html-tag.gif)


##1- Linking to Other Sites:
Links are created using the `<a>` element which has an attribute
called href. The value of the href attribute is the page that
you want people to go to when they click on the link.


```<p>Movie Reviews:
<ul>
<li><a href="http://www.empireonline.com">
Empire</a></li>
<li><a href="http://www.metacritic.com">
Metacritic</a></li>
<li><a href="http://www.rottentomatoes.com">
Rotten Tomatoes</a></li>
<li><a href="http://www.variety.com">
Variety</a></li>
</ul>
</p>
```
##2- Linking to Other Pages on the Same Site:

When you are linking to other pages within the same site,
you do not need to specify the domain name in the URL. You
can use a shorthand known as a **relative URL**.



``` <p>
<ul>
<li><a href="index.html">Home</a></li>
<li><a href="about-us.html">About</a></li>
<li><a href="movies.html">Movies</a></li>
<li><a href="contact.html">Contact</a></li>
</ul>
</p>
```
**Relative URLs:** When linking to other pages within the same site, you can use relative URLs. These are like a shorthand version of absolute URLs because you do not need to specify the domain name.

## 3- Email Links:
**mailto**: email-links.html HTML to create a link that starts up the user's email program and addresses an email to a specified email address, you use the `<a>` element. However, this time the value of the href attribute starts with mailto: and is followed by the email address you want the email to be sent to.

`<a href="mailto:jon@example.org">Email Jon</a>`

### Opening Links in a New Window:
**target**
If you want a link to open in a new window, you can use the target attribute on the opening `<a>` tag. The value of this attribute should be _blank.


## Building Blocks:
CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.
Block-level boxes start on a new line and act as the main building blocks of any layout, while inline boxes flow between surrounding text. You can control how much space each box takes up by setting the width of the boxes (and sometimes the height, too). To separate boxes, you can use borders, margins, padding, and background colors.
 ![](https://media.gcflearnfree.org/content/5ef2084faaf0ac46dc9c10be_06_23_2020/box_model.png)
 
 ## What is JavaScript Functions:

A JavaScript function is a block of code designed to perform a particular task.
A JavaScript function is executed when “something” invokes it (calls it).


``function name(parameter1, parameter2, parameter3) {
// code to be executed
}
 ``
 we can declare a functions that need a `parameter`

## Pair programming

 While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.