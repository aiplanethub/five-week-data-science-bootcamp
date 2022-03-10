# Multiple Plots

### Multiple Plots in 1 Figure

* We can make multiple graphics in one figure. This goes very well for comparing charts or for sharing data from several types of charts easily with a single image.\

* The .subplot() method is used to add multiple plots in one figure. It takes three arguments:
  * nrows: number of rows in the figure
  * ncols: number of columns in the figure
  * index: index of the plot\

* Let's see how variables are plotted with different row and column configurations in the figures.\

* The function subplot creates a figure and a set of subplots. It is a wrapper function to make it convenient to create common layouts of subplots, including the enclosing figure object, in a single call.\

* You can even give a Title to your subplots using the suptitle method! No, the 'p' is not a typing mistake.\

* The subplot function returns a figure and an Axes object or an array of Axes objects.

### Changing Plot Size

If we call the subplot function without any parameters - like we do in the following example - a Figure object and one Axes object will be returned:

![](https://lh6.googleusercontent.com/T-MBLEeJb3CIqBysfMsTFE8S0x7DfGwfBR96fYza1Kp3ghWSAoAjnG41iEJHgkfMkwaFaaUsRDsHGmNUg6tNdZvqjtiWoGk2XSEiLowfJWge8Xg8xJJ93hdZVwCcX8tOKdJMQONx9YE=s0)

### 1 row and 2 columns - Method 1

![](https://lh3.googleusercontent.com/SlhKyw\_CNDzPZ1dJB5\_BwWTHltOhOwhAl8q2qj6DL0tK7FrP1XVaafas7SGmgaOgu7bfYZBCoa2NyWNA6IYmED1FJVYuYTqFE7mdzjTEsbcLgxe6K3FgVTaFu0SaeKr-QkR9up18N9Y=s0)

### **1 row and 2 columns - Method 2**

![](https://lh6.googleusercontent.com/LnTP38A6blHMXEAk1bHkCrl171glAKWrkD16ZJCuuS2KNWOmTy843EV9B2UmTbE0MyJ5txJFwFaThEzaBzI8v\_d48OGW4gKbhgncIiz5ufuB7-BlD1YSAdS4pWazhMzYHjEEFD8W3wA=s0)

### Overlapping Values

* PS. Aren't those overlapping axis values annoying? Matplotlib has a solution for that too. \

* Simply put sharey=True inside the subplot function. The two subplots will share the y axis values then. \

* Try it out!

### 2 rows and 1 column

![](https://lh4.googleusercontent.com/3X-CycTu\_r7ETKuBhu8880ufkZ9aZXFGabokvaG5sz0ZCm-tXf3SORBUvllfaJRVVOvbbuDypQI4Ag2LFclAhPaYPwNpc0ARAPrL81Qmdv-AF64E\_qiroFuNOvfy8tyaK3uCEthR9U0=s0)



### 2 rows and 2 columns

Think of this as a 2X2 grid. You can access the different positions of the axis and plot your graphs there as follows:

![](https://lh3.googleusercontent.com/B7J5O2\_wtFHiR\_BSc3F6WX7TWT5BZykEkdmWPnVKOIBGduPEWdW4nmT7jaJmUHB1zwUrCAWLs29oNcJ6mJhb-4k\_1h\_5X1DNhRI9ExkgENCoIvG8qC9c9Qm51lJJzC1dTF3lqPqxDkg=s0)
