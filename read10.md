## Lists:
**Ordered lists:** are lists where each item in the list is numbered. For example, the list might be a set of steps for a recipe that must be performed in order, or a legal contract where each point needs to be identified by a section number.

 The ordered list is created with the `<ol>` element.
 `<li>`
Each item in the list is placed between an opening `<li>` tag and a closing `</li>` tag. (The li stands for list item.)

``` <ol>
<li>Chop potatoes into quarters</li>
<li>Simmer in salted water for 15-20
minutes until tender</li>
<li>Heat milk, butter and nutmeg</li>
<li>Drain potatoes and mash</li>
<li>Mix in the milk mixture</li>
</ol> 
```









●● **Unordered lists:** are lists that begin with a bullet point (rather than characters that indicate order).
`<ul>`
The unordered list is created with the `<ul>` element.

``` <ul>
<li>1kg King Edward potatoes</li>
<li>100ml milk</li>
<li>50g salted butter</li>
<li>Freshly grated nutmeg</li>
<li>Salt and pepper to taste</li>
</ul>
```

●● **Definition lists:** are made up of a set of terms along with
the definitions for each of those terms.
`<dl>`
The definition list is created with the `<dl>` element and usually consists of a series of terms and their definitions. Inside the `<dl>` element you will usually see pairs of `<dt>` and `<dd>` elements

``` <dl>
<dt>Sashimi</dt>
<dd>Sliced raw fish that is served with
condiments such as shredded daikon radish or
ginger root, wasabi and soy sauce</dd>
<dt>Scale</dt>
<dd>A device used to accurately measure the
weight of ingredients</dd>
<dd>A technique by which the scales are removed
from the skin of a fish</dd>
<dt>Scamorze</dt>
<dt>Scamorzo</dt>
<dd>An Italian cheese usually made from whole
cow's milk (although it was traditionally made
from buffalo milk)</dd>
</dl>
```
`<dt>`
This is used to contain the term being defined (the definition term).
`<dd>`
This is used to contain the definition. Sometimes you might see a list where there are two terms used for the same definition or two different definitions for the same term.


## Boxes:
#### width, height:
By default a box is sized just big enough to hold its contents. To set your own dimensions for a box you can use the height and width properties. The most popular ways to
specify the size of a box are to use pixels, percentages, or ems. Traditionally, pixels have been the most popular method because they allow designers to accurately control their size.


``` div.box {
height: 300px;
width: 300px;
background-color: #bbbbaa;}
p {
height: 75%;
width: 75%;
background-color: #0088dd;}
```



### Border, Ma rgin & Padding:
![describing](https://i.pinimg.com/originals/f6/f6/c9/f6f6c946356774ddb886956cd94df4c9.png)

##### Border
Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another.
##### Margin
Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.
##### Padding 
Padding is the space between the border of a box and any
content contained within it. Adding padding can increase the
readability of its contents.



## Loops:
### for loops:
A for loop is often used to loop through the items in an array. In this example, the scores for each round of a test are stored in an array called scores. The total number of items in the array is stored in a variable called array l  ength. This number is obtained using the length property of the array.

```//Loop through the items in the array
for (i = O; i < arraylength; i++) {
//Arrays are zero based (so 0 is round 1)
//Add 1 to the current round
roundNumber = (i + l);
// Write the current round to message
msg += 'Round ' + roundNumber + ' : ';
//Get the score from the scores array
msg += scores[i] + '<br / >' ;
```
### While loops:
Here is an example of awhile loop. It writes out the 5 times table. Each time the loop is run, another calculation is written into the variable called msg. This loop will continue to run for as long as the condition in the parentheses is true. That condition is a counter indicating that, as long as the variable i remains less than 10, the statements in the subsequent code block should run.



II Store 5 times tabl e in a variable
```while (i < 10) {
msg += i + ' x 5 = ' + (i * 5) + '<br I>';
i++;
```


### Arrays:
An array is a special type of variable. It doesn't just store one value; it stores a list of values.

``` var colors;
colors ['white', 'black', ' custom '];
var el document.getElementByld('col ors');
el . textContent = col ors[O];
```
