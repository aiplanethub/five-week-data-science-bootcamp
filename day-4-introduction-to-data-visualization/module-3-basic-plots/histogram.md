# Histogram

### What is **Histogram?**&#x20;

A histogram is a graphical display of data using bars(rectangles) of different heights.

**Parts of a Histogram:**

* **The title:** The title describes the information included in the histogram.
* **X-axis:** The X-axis are intervals that show the scale of values which the measurements fall under. These intervals are also called bins.
* **Y-axis:** The Y-axis shows the number of times that the values occurred(frequency) for each interval on the X-axis.
* **The bars:** The height of the bar shows the number of times that the values occurred within the interval, while the width of the bar shows the interval that is covered.

### **Example: Height of Orange Trees**

* You measure the height of every tree in the orchard in centimeters (cm)
* The heights vary from 100 cm to 340 cm
* You decide to put the results into groups of 50 cm:
  * The 100 to just below 150 cm range,
  * The 150 to just below 200 cm range, Etc…
* So a tree that is 260 cm tall is added to the "250-300" range.

![](https://lh5.googleusercontent.com/15xqYxG9h5snjcXxgH3pPplNxh7kQdD4zsnluS6N-6L3QhsRKmJ4TYFwBxlhx7wsTjnGevYRqkBCYHMvkFv0eeVMEdzF9W\_iXOPtK83-mjpE2w5IcO4jZY9teKVmNzH\_nBKJ1D0OwBk=s0)

* **And here is the result:**&#x20;

![](https://lh3.googleusercontent.com/i1a-OvjJh-AmC0fO5rJI\_pdz4X6vII\_DAHJowHPTqbBn\_lomzG7ppU5jxibTufIfWSA\_xlwz4iSK6J4Vu\_7LvxDmbRG9oqIkcfsZp9LC9n39qU94\_-E9T50QzMRLZIYZ6N4-SZVwjLo=s0)

* You can see (for example) that there are 30 trees from 150 cm to just below 200 cm tall. You just created a histogram!
* Source: https://www.mathsisfun.com/data/histograms.html

### Creating a Histogram&#x20;

Matplotlib can be used to create histograms using the hist() method.&#x20;

Parameters:

* x(n,) : this takes either a single array or a sequence of arrays which are not required to be of the same length.
* bins : intervals of any quantity

If the bins are:&#x20;

\[1, 2, 3, 4]

then the first bin is \[1, 2) (including 1, but excluding 2) and the second \[2, 3). The last bin, however, is \[3, 4], which includes 4.\


![](https://lh3.googleusercontent.com/4b5vWDWb\_vKczyxCW15jBttrCHm5PJ8eNOpnBiPKOpPVjIp-l0eRanZjJsyEzCQX-fd6G6wK4S6fw8t2B6Ib5AE6xhgSUNObHHctQbSxYDzANVUKxniJubMuspXYY-33Z\_KroTxKrRI=s0)

### **Applications of Histogram**&#x20;

* Histograms are a very common type of plots when we are looking at data like height and weight, stock prices, waiting time for a customer, etc which are continuous in nature.
* Histograms are good for showing general distributional features of dataset variables. You can see roughly where the peaks of the distribution are, whether the distribution is skewed or symmetric, and if there are any outliers.
