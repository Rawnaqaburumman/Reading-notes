# TEXT: 
**Tags Or markup:** provide extra meaning and allow browsers to show users the appropriate structure for the page.
It devided into :
* **Structural markup**: the elements that you can use to describe both headings and paragraphs.
* **Semantic markup**: which provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it), the meaning of acronyms, and so on.There are some text elements that are not intended to affect the structure of your web pages, but they do add extra information to the pages.

## Headings :
HTML has six "levels" of headings:

 ```<h1>This is a Main Heading</h1>
<h2>This is a Level 2 Heading</h2>
<h3>This is a Level 3 Heading</h3>
<h4>This is a Level 4 Heading</h4>
<h5>This is a Level 5 Heading</h5>
<h6>This is a Level 6 Heading</h6>
```


<h1>This is a Main Heading</h1>
<h2>This is a Level 2 Heading</h2>
<h3>This is a Level 3 Heading</h3>
<h4>This is a Level 4 Heading</h4>
<h5>This is a Level 5 Heading</h5>
<h6>This is a Level 6 Heading</h6>

## paragraphs:
To create a paragraph, surround the words that make up the paragraph with an opening `<p>` tag and closing `</p>` tag. By default, a browser will show each paragraph on a new line with some space between it and any subsequent paragraphs.

 `<p> Text is easier to understand when it is split up into units of text. For example, a book may have chapters. Chapters can have subheadings. Under each heading there will be one or more paragraphs.</p>
`

## Bold & Italic:
 By enclosing words in the tags` <b> `and `</b>` we can make characters appear bold. 
By enclosing words in the tags `<i>` and `</i>` we can make characters appear italic.

## Superscript & Subscript:
The `<sup>` element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power such as 22.

The `<sub>` element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H20.

## Line Breaks & Horizontal Rules:
if you wanted to add a line break inside the middle of a paragraph you can use the line break tag `<br />`.

## Strong & Emphasis:
The use of the `<strong>` element indicates that its content has strong importance. For example, the words contained in this element might be said with strong emphasis. By default, browsers will show the contents of a `<strong>` element in bold.

## Abb reviations & Acronyms:
If you use an abbreviation or an acronym, then the `<abbr>`or `<acronym>` element element can be used. A title attribute on the opening tag is used to specify the full term.

## Citations & Definitions:

`<cite>`
When you are referencing a piece of work such as a book, film or research paper, the <cite> element can be used to indicate where the citation is from.

`<dfn>`
The first time you explain some new terminology (perhaps an academic concept or some jargon) in a document, it is known as the defining instance of it.


## Introducing CSS:
CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented. CSS works by associating rules with HTML elements. These rules govern ow the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.

 Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties. For example, the font-family property sets the choice of font, and the value arial specifies Arial as the preferred typeface.

 ## Basic JavaScript Instructions:
 A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a **statement**. Statements should end with a semicolon.

 ### Variables:
 A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.
 varibles can be decleared using :Var or let.

 ### ARRAYS:
 An array is a special type of variable. It doesn't just store one value; it stores a list of values.

 `Bar colors;
colors =['white', 'black', ' custom '];`

### EXPRESSIONS
An expression evaluates into (results in) a single value. Broadly speaking there are two types of expressions: 
- EXPRESSIONS THAT JUST ASSIGN AVALUE TO A VARIABLE
- EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE
