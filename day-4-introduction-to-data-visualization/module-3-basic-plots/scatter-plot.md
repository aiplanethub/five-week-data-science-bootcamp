# Scatter Plot

### What is Scatter Plot?

* A scatter plot (aka scatter chart, scatter graph) uses dots to represent values for different numeric variables.
* The position of each dot on the horizontal and vertical axis indicates values for an individual data point.
* Scatter plots are used to observe relationships between variables.

![](https://lh4.googleusercontent.com/gDA20fCb-aGaID3zbDNlqcvM\_8mej0keUsfLLDu3mOM52Jr6aJerWNHfw5P71ZEJ1DI51JYqR-XKeXQtMIZzW1QSegV7kK831IANBgLHeCCygn6WUHM9E7D812tCXIR0OPxsnaynoMo=s0)

### **Creating a Scatter Plot**

To create a scatter plot in Matplotlib we can use the .scatter() method:

![](https://lh3.googleusercontent.com/BLN9atPgko8o28-xinFlBNveX1COkebSv-wG9D6M99-qlP5VESbZXlDAhkGghdprSvLIVg-M8PRqEyOluRygi92QOi5W2bQpigjq4wGlFobnCNzipInLcfgvmdu3o78xtOoUSf5\_-Mw=s0)

### **Is plt.show( ) always required?**

You might’ve observed the line plt.show( ) after the plt.scatter( ). Is it necessary to use?

* If Matplotlib is used in a terminal, scripts or specialized IDEs such as Spyder, Pycharm or VS Code, plt.show() is a must.
* If Matplotlib is used in a IPython shell or a notebook as Jupyter Notebook or Colab Notebook, plt.show() is usually unnecessary.

The plt.show() command does a lot under the hood, as it must interact with your system's interactive graphical backend. The details of this operation can vary greatly from system to system and even installation to installation, but matplotlib does its best to hide all these details from you.

In the following cell we are executing the same script as above, removing the plt.show() instruction:

![](https://lh6.googleusercontent.com/ca9aAa7Tus66y5tSUTNY8DQK70b7rTCP33c\_Ke9J6eX3mEC3WyMr8ZiORWghMwPO3HGbyTFqDGVJFEJDKiEMNxpBy8FuzI7EnlID2dtiMOdCiGXZdyrgTlsOKF2QlZe\_1pLE6U7OwHI=s0)

If you want to prevent this from being included as a cell output, use plt.show() at the end of each plotting instruction.

### **Applications of Scatter Plot**

* A scatter plot can be useful for identifying other patterns in data.
* We can divide data points into groups based on how closely sets of points cluster together.
* Scatter plots can also show if there are any unexpected gaps in the data and if there are any outlier points. (Look at the 2 points away from rest of the data in the scatter plot. Those are outliers.)
* This can be useful if we want to segment the data into different parts, like categorising users into different groups.
