# Building Blocks CSS:
CSS treats each HTML element as if it is in itsown box. This box will either be a block-level box or an inline box.
Containing Elements
 If one block-level element sits inside another block-level element then the outer box isknown as the containing or parent element.
It is common to group a number of elements together inside a <div> (or other block-level) element. For example, you might group together all of the elements that form the header of a site (such as the logo and the main navigation). The <div> element that contains this group of elements is then referred to as the containing element.




CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.
 - Normal flow
 - Relative Positioning
 - Ab solute positioning


 The float property allows you to take an element in normal flow and place it as far to the left or right of the containing
element as possible. Anything else that sits inside the containing element will flow around the element that is floated.
- left
- right
- both
- none

The liquid layout uses percentages to specify the width of each box so that the design will stretch to fit the size of thescreen.
When trying this in your browser, remember to make the window smaller and larger. 


Designers keep pages within 960-1000 pixels wide,and indicate what the site is about within the top 600
pixels (to demonstrate its relevance without scrolling).

![](https://i.stack.imgur.com/SmUG9.png)