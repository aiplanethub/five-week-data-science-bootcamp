# Formatting The Plots

### Learning Objectives

* Changing Colors
* Changing line-styles
* Adding Markers
* Combining the 3 formatting option

### Formatting Plots

* The first adjustment you might wish to make to a plot is to control the line colors and styles.\

* Look at all the above graphs you’ve created till now. What is the color and style of the plots where it is not explicitly specified? \

* **All blue solid lines. Blue solid line is thus the default formatting style.**\
  ****
* The plt.plot() function takes additional arguments that can be used to specify the formatting.\

* You've already specified the colour of a few plots before using the 'color' argument. Colours can be provided in a number of ways apart from that.

### 1. Changing Colours

To adjust the color, you can use the color keyword, which accepts a string argument representing virtually any imaginable color. The color can be specified in a variety of ways:

![](https://lh3.googleusercontent.com/XrZFU1P6LGfJtszx83YzFy1onqFw9FkkroMxoJYMVx3YZ5UZriezgq4r7-t3Rm6SuqiRTkisUitFvI6cGl37ylDaBWRIAnvlWWFH26aXDUjxn3kyCmsL5qw42wCvMm-OkQnjoVta0Yg=s0)

If no color is specified, Matplotlib will automatically cycle through a set of default colors for multiple lines.

### 2. Changing Line Styles

Similarly, the line style can be adjusted using the linestyle keyword. You can make the lines dashed, dotted or a combination of both.

![](https://lh4.googleusercontent.com/710Q3smnAgXDyBI0Bp73YmCY2WBwUtMdAbqnfgMYlpz\_kTUws3tTGGtg9WV83gFNG5fRDh096HigsZViXq-gCUt-nUL-Icj6ZP3iiYgrD8Nt0kZb-YLyzV-vmjjLP8EUotk8RpfT1hM=s0)

### 3. Adding Markers

So you've plotted lines that pass through the points in the dataset. But we can't really see those points in the lines above, can we?

Adding markers to a line plot can be a useful way to distinguish multiple lines or to highlight particular data points.&#x20;

![](https://lh6.googleusercontent.com/lplrE0fE5E9zXzILnWZDg-Lz5yAEoSDYZqH6RIjN0u7w-nE\_KisDcaihsHgDzLaFDcKRQSkbc4ozo0-1V8CMoiujyFSz6cKt-\_PZu-D\_rZoi9ebMXdGKnSXs9I9kSi2DqVSJDgqZ6uA=s0)



### Combining the 3 formatting options

Let's plot a red dashed line with triangular markers!

![](https://lh4.googleusercontent.com/2uMAc9j6wVWHV1Kcv-43fQV\_btc3SOc6oEWqIxSZVrEA05ToRrcjNMKVv6B5d25\_8M-O14eIHYciziD5rDq-9Ixaep8wT9E7Z1wAwXQ4xABPde0PcFIoLySxLcmz0Zr0kvUVf-e-eZk=s0)

### Shortcut for above

For every x, y pair of arguments, there is an optional third argument which is the format string that indicates the color and line type of the plot. The letters and symbols of the format string are from MATLAB, and you concatenate a color string with a line style string. The default format string is 'b-', which is a solid blue line.

These linestyle and color codes can be combined into a single non-keyword argument to the plt.plot() function:

![](https://lh6.googleusercontent.com/blLNAzk3\_1WjGxM5NsC\_EaBtvn6L8LMM2q1eYSRutfErYePemQ2TyiSlHpI9CIizJb7lOJsN\_VlLq9NT0M8xypwVC5JPZSgSLY3ys\_0PAvKFKTzMfaMumvfie-0DD8nYFjnQrakgFWE=s0)

### Scatter Plot with plot function

It turns out that the plot function can produce scatter plots as well. Just don't mention any linestyle.

![](https://lh3.googleusercontent.com/pLGECu1H5W63CWk\_N9HzWdclEzU4usRQMZFwPuDMvvoO0kc2tAoTPr3stgycaDxEqiMzFVrzd9-NxAhS373lVapY9-ob-WDe1Kj4vf2lsxJ-HX8dvuBJhmt-tMpsa8uvjsIXFwCixyM=s0)

### More examples

![](https://lh3.googleusercontent.com/ritjOjYLYQ-j4FpR6HlYt0Sr0AUyLtqrSXMD\_E\_w-jVki8AQfHeely-mBMlO2Oa\_2lrxKhyFJ-4sTM-KRdIecs7bc7GGhVtFKKqWigfP\_92nGrLH5iJWvaR7EP1oXnMWOIF8Ey8gJtA=s0)

There are plenty of other options. You can try the following:

![](https://lh4.googleusercontent.com/ri8sw5I5Lv7W1tqL3h0knKRXxQqlrYuVH2T28uHjCJnkpE24tUznVVl9\_ad9XhBomjyqdLwOCT\_JYe566i2IV72LKN8\_7277RdULpr4TAZSCMd634NvRN3FYbZEacVlnx\_06BaCvM-I=s0)

These single-character color codes reflect the standard abbreviations in the RGB (Red/Green/Blue) and CMYK (Cyan/Magenta/Yellow/blacK) color systems, commonly used for digital color graphics.
