# Images:

### Storing Images on Your Site :
images are stored in a folder called images.

### Adding Images :
`<img>`
To add an image into the page you need to use an <img> element. This is an empty element (which means there is no closing tag). It must carry the following two attributes:

`<img src="images/quokka.jpg" alt="A family of
quokka" title="The quokka is an Australian
marsupial that is similar in size to the
domestic cat." />`

#### height
This specifies the height of the image in pixels.
#### width
This specifies the width of the image in pixels.

Figure and Figure Caption:
`<figure>`
Images often come with captions. HTML5 has introduced a new `<figure>` element to contain images and their caption so that the two are associated. You can have more than one image inside the `<figure>` element as long as they all share the same caption.

# Color:
The color property allows you to specify the color of text inside
an element. You can specify any color in CSS in one of three ways:

**rgb values**
These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90).

**hex codes**
These are six-digit codes that represent the amount of red,
green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80.

**color names**
There are 147 predefined color names that are recognized
by browsers. For example: DarkCyan.

![](https://raw.githubusercontent.com/ap/vim-css-color/5377c65022ee6d660b898bad954aeea73fa613b8/screenshot.png)

##### background-color:
CSS treats each HTML element as if it appears in a box, and the
background-color property sets the color of the background for that box.
![](https://i.stack.imgur.com/6fkyP.png)


# Text:
#### Typeface Terminology:
![](https://www.designmantic.com/blog/wp-content/uploads/2015/09/Typeface-Glossary-Banner.jpg
)
- Serif
- Sans-Serif
- Monospace

##### Techniques That Offer a Wider Choice of Typefaces:
- font-family
- font-face
- Service-based Font-Face


#### JPEG vs PNG vs GIF — which image format to use and when?
### TL;DR
Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use GIF format for images that contain animations.

### Compression
Almost all forms of data that we see on the internet — text, image, video etc. — are compressed to reduce the size of data and ensure faster transmission. Choosing the correct format and compression is a major factor that determines image size

### PEG 
is a lossy compression specification that takes advantage of human perception. It can achieve compression ratios of 1:10 without any perceivable difference in quality

