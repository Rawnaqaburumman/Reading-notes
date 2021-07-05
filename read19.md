# Charts :
A great way to get started with charts is with **Chart.js**, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.


### Setting up
The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script:



``` <!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8" />
        <title>Chart.js demo</title>
        <script src='Chart.min.js'></script>
    </head>
    <body>
    </body>
</html>
```
### Installation
You can get the latest version of Chart.js from npm , the GitHub releases , or use a Chart.js CDN . Detailed installation instructions can be found on the installation page.


It's easy to get started with Chart.js. All that's required is the script included in your page along with a single `<canvas>` node to render the chart.


###  Drawing text:
The canvas rendering context provides two methods to render text:

fillText`(text, x, y [, maxWidth])`
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
strokeText(text, x, y [, maxWidth])
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
