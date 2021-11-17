# Matplotlib tutorial

- matplotlib: is probably the single most used Python package for 2D-graphics. It provides both a very quick way to visualize data from Python and publication-quality figures in many formats. We are going to explore matplotlib in interactive mode covering most common cases.
- IPython and the pylab mode : is an enhanced interactive Python shell that has lots of interesting features including named inputs and outputs, access to shell commands, improved debugging and much more. When we start it with the command line argument -pylab (–pylab since IPython version 0.12), it allows interactive matplotlib sessions that have Matlab/Mathematica-like functionality.
- pyplot : provides a convenient interface to the matplotlib object-oriented plotting library. It is modeled closely after Matlab(TM). Therefore, the majority of plotting commands in pyplot have Matlab(TM) analogs with similar arguments. Important commands are explained with interactive examples. 

## seaborn tutorial

- Seaborn : is a library for making statistical graphics in Python. It is built on top of matplotlib and closely integrated with pandas data structures.

- Here is some of the functionality that seaborn offers:

   -  A dataset-oriented API for examining relationships between multiple variables

    - Specialized support for using categorical variables to show observations or aggregate statistics

    - Options for visualizing univariate or bivariate distributions and for comparing them between subsets of data

    - Automatic estimation and plotting of linear regression models for different kinds dependent variables

    - Convenient views onto the overall structure of complex datasets

    - High-level abstractions for structuring multi-plot grids that let you easily build complex visualizations

    - Concise control over matplotlib figure styling with several built-in themes
    -
    
```
install matplotlib

```
### Import Matplotlib
Once Matplotlib is installed, import it in your applications by adding the import module statement:

```
import matplotlib
```
Now Matplotlib is imported and ready to use:

## Matplotlib Pyplot

### Pyplot
Most of the Matplotlib utilities lies under the pyplot submodule, and are usually imported under the plt alias:

```
import matplotlib.pyplot as plt
```
Now the Pyplot package can be referred to as plt.

### Example
Draw a line in a diagram from position (0,0) to position (6,250):

```
import matplotlib.pyplot as plt
import numpy as np

xpoints = np.array([0, 6])
ypoints = np.array([0, 250])

plt.plot(xpoints, ypoints)
plt.show()
```
### Result:

![0](https://www.w3schools.com/python/img_matplotlib_pyplot.png)

## Matplotlib Plotting

### Plotting x and y points
The plot() function is used to draw points (markers) in a diagram.

By default, the plot() function draws a line from point to point.

The function takes parameters for specifying points in the diagram.

Parameter 1 is an array containing the points on the x-axis.

Parameter 2 is an array containing the points on the y-axis.

If we need to plot a line from (1, 3) to (8, 10), we have to pass two arrays [1, 8] and [3, 10] to the plot function.

### Example

Draw a line in a diagram from position (1, 3) to position (8, 10):

```
import matplotlib.pyplot as plt
import numpy as np

xpoints = np.array([1, 8])
ypoints = np.array([3, 10])

plt.plot(xpoints, ypoints)
plt.show()
```

### Result:

![1](https://www.w3schools.com/python/img_matplotlib_plotting1.png)
