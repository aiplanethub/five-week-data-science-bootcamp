# Day 3: More on Statistics, Data Cleaning & EDA

### Learning Objectives

* Distribution
* Skewness
* Practise Data Cleaning

### **Distribution**

* **Probability** - by going with the literal meaning it is the extent to which something is likely to happen or probable. The same concept applies to statistics when we talk about probability distributions.
* A **probability distribution** is a function that describes the likelihood of obtaining the possible values (probability) of a variable.
* **Suppose a teacher** notes down the heights of all students in her class.
* Now, she can draw a probability distribution when she needs to know which outcomes (heights) are most likely, the spread of potential values (range of heights), and the likelihood of diﬀerent results (probability of each height).

### Distribution

* Let’s take the heights dataset consisting of student IDs and heights: [https://bit.ly/Heights\_Data](https://bit.ly/Heights\_Data)&#x20;
* The most convenient way to take a quick look at a distribution in seaborn is the displot() function. On plotting a distplot on this dataset, we’ll observe a bell shaped curved like this:

&#x20;                      &#x20;

![](https://lh6.googleusercontent.com/jtyG1w3AP5tUrDwbASZDC0JlWqkjClsbhzGMRtMaEBXihiRyOZI9E4cCV7S1FeL29FP3t9TzjHO82\_khGO6I5yKdG8BOvF42PbhVabTggd8TkgABAd1fOZmNkJaBc9sl-XeQp80heTI)

* Probability distributions are usually (but not solely) represented in charts whose abscissa axis ( x axis) represents the possible values of the variable and whose ordinal axis ( y axis) represents the probability of occurrence (probability density).

![](https://lh4.googleusercontent.com/W0rb9xh15ItGdPMJFUzxHsR5xW6zOH3LD7lWdx7ZnnAm\_-0mQWbhpj0IiR6LQa1iHL2UoaV8yfHwCYAe8jk6amEXA\_h\_97n7P7Yry-z5WMvLkdWN3bKFufKdX4R8CwtOBxEZjBsO1Nw)

* Most statistical models rely on a normal distribution, a distribution that is symmetric and has a characteristic bell shape.

### Normal / Gaussian Distribution

* Also called bell shaped curve.

![](https://lh4.googleusercontent.com/Jody1mGfE60Q3zETPTWIt8TJktwdn3xomB9lpjEsaEopiwKd-EsUqKGAlb1xo\_hYVEGUVL3FZ9NAabbHKSUIkp4v4FnawKWJJ8WUVmtYUYN5W71KT7ors6xNIJhpwxm8-IlX0OKrziw)

* It is a distribution of data that occurs naturally in many situations.
* It is a probability distribution that is symmetric about the mean, showing that data near the mean are more frequent in occurrence than data far from the mean.

{% embed url="https://www.youtube.com/watch?v=iMak-EW4HtM" %}

### Skewness

* Real life data rarely, if ever, follow a perfect normal distribution.
* The skewness measures the symmetry of a distribution or how diﬀerent a given distribution is from a normal distribution.
* The normal distribution is symmetric and has a skewness of zero.

### Types of Skewness

* There are two types of Skewness: Positive and Negative

![](https://lh6.googleusercontent.com/FePiK28orBBwiysvmbgmLz0alqhwY6xItYaxxuWLR9HtC9ZyhwxMeOaSHpOngpDykeaHFnYt0OfIwCJ2z3cDNfWvh\_kZUWyacisZK1F0cTrXw4oSqaVqY8aq-\_d1mzMVDxULGjOU\_xM)

* **Positive/Right Skewness** means when the tail on the right side of the distribution is longer or fatter. The mean and median will be greater than the mode.
* **Negative/Left Skewness** is when the tail of the left side of the distribution is longer or fatter than the tail on the right side. The mean and median will be less than the mode.
* **For further reading refer:** [https://www.statisticshowto.com/probability-and-statistics/skewed-distribution/](https://www.statisticshowto.com/probability-and-statistics/skewed-distribution/)

### Understanding skewness with an example

* Let us take a very common example of house prices. Suppose we have house values ranging from $100k to $1,000,000 with the average being $500,000.
* If the peak of the distribution was left of the average value, portraying a positive skewness in the distribution. It would mean that many houses were being sold for less than the average value, i.e. $500k. This could be for many reasons, but we are not going to interpret those reasons here.
* If the peak of the distributed data was right of the average value, that would mean a negative skew. This would mean that the houses were being sold for more than the average value.

### Data Cleaning Practice

Time for getting your hands dirty and cleaning a dataset!

Follow the various steps of Data Cleaning in this article to clean the Russian Housing Dataset. It covers everything we’ve learnt till now.

You’ll analyse and visualise data, detect outliers, remove irrelevant and inconsistent values and get a structured, clean data at the end.

* [https://towardsdatascience.com/data-cleaning-in-python-the-](https://towardsdatascience.com/data-cleaning-in-python-the-ultimate-guide-2020-c63b88bf0a0d) [ultimate-guide-2020-c63b88bf0a0d](https://towardsdatascience.com/data-cleaning-in-python-the-ultimate-guide-2020-c63b88bf0a0d)
