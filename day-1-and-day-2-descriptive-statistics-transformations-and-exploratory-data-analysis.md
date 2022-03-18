# Day 1 & Day 2: Descriptive Statistics, Transformations and Exploratory Data Analysis

### Learning Objectives

* Measures of Dispersion
* Transformations
* EDA with Seaborn
* Additional Python Topics

### **Measures of Dispersion**

* **Range:** It is the diﬀerence between highest value and the lowest value in the data set. \
  For a given list of numbers: 10, 20, 40, 10, 70 the range is 70 - 10 = 60.\

* **Variance:** The average of the squared diﬀerences from the mean. Steps to calculate variance:
  * Calculate mean (mean is nothing but average)
  * Find diﬀerence of each data from mean
  * Square all the diﬀerences
  * Take the average of the squares.\

* **Standard Deviation:** It shows you how much your data is spread out around the mean. Its symbol is 𝛔 (the greek letter sigma). It is the square root of the **variance.**     &#x20;

### **Standard Deviation**                                           &#x20;

{% embed url="https://www.youtube.com/watch?v=heN3uvJ99Vo" %}

### Calculate Variance

**Steps to calculate variance:**

* Calculate mean
* Find diﬀerence of each data from mean
* Square all the diﬀerences
* Take the average of the squares.

Consider the list of numbers: 10, 20, 40, 10, 70.

* Mean of the number is 30.
* Diﬀerence of each data from the mean: -20, -10, 10, -20, 40.
* Square of all the diﬀerences: 400, 100, 100, 400, 1600
* Take the average of the squares: (400 + 100 + 100 + 400 + 1600) / 5 = 2600 / 5 = 520

### Standardization / Normalization

* Often variables in a real dataset come with a wide range of data values.
* **For example** let’s look at the wine dataset given in next slide, the **ﬁxed.acidity variable has values ranging from 3.8 to 14.2**.&#x20;
* Similarly, if we look at **volatile.acidity, it has values ranging from 0.08 to 1.10**. Basically, they are not on a common scale.

**Now how does standardization/normalization help?**

* Performing standardization/normalization would bring all the variables in a dataset to a common scale so that it could further help in implementing various machine learning models (where standardization/normalization is a pre-requisite to apply such models).&#x20;
* Again, don’t take this for granted, there are some smart algorithms which doesn’t need this and we will explore them soon!

![](https://lh6.googleusercontent.com/YBk3tz1PnkS\_nzn7SLreBdeVBAO0pCzAU-E1TFfwQI2kCiiHWxuRJVpHBX3lcWM7nVTdHgWG\_wfCYz8vkXe8Pz6Tf1X9\_VEPQi1pKr0-PEcJcnwrmolmhAg1be4mBlEJR0PRiLRM14k)

![](https://lh3.googleusercontent.com/03Lp-HdY1nGIQHATpYl97ZFxlPoseACRfdj\_HXVqgpDZ0RXDHCdZDXm\_JIf3txnSptArHEDF8fu4dP2nHpdW-rb\_q6KN5Y\_NC\_ERiwJFAcJKb9o6jq6KyXnTes2nrEkzasp3ScIxjv8)

* Look at the above graphs. The actual data is scattered across a wide range.
* Normalisation helps in bringing the whole data within a particular range.
* Standardisation distributes the data in a manner such that it now has a mean of 0 and standard deviation of 1.

### Transformation

Some machine learning algorithms are quite sensitive to the scale of the numeric values provided.

Consequently, in order for the algorithm to converge faster or to provide a more exact solution, rescaling the distribution is necessary. Rescaling mutates the range of the values of the features and can aﬀect variance, too. You can perform features rescaling in two ways:

* Using statistical **standardization** (z-score normalization): \
  Standardization typically means rescaling data to have a mean of 0 and a standard deviation of 1 (unit variance).
* Using the min-max transformation (or **normalization**):\
  Normalization typically means rescaling the values into a range of \[0,1].

### EDA with Seaborn

In today’s session, we’ll be performing EDA by visualising data with Seaborn (speciﬁcally with scatterplot, countplot, distplot, boxplot and heatmap).

Please go through the following material to understand these diﬀerent plots:

[https://towardsdatascience.com/how-to-perform-exploratory-data-analysis-wit](https://towardsdatascience.com/how-to-perform-exploratory-data-analysis-with-seaborn-97e3413e841d)[h-seaborn-97e3413e841d](https://towardsdatascience.com/how-to-perform-exploratory-data-analysis-with-seaborn-97e3413e841d)

[https://towardsdatascience.com/analyze-the-data-through-data-visualization-us](https://towardsdatascience.com/analyze-the-data-through-data-visualization-using-seaborn-255e1cd3948e)[ing-seaborn-255e1cd3948e](https://towardsdatascience.com/analyze-the-data-through-data-visualization-using-seaborn-255e1cd3948e)

### **Additional Python Topics (Optional)**

**(This is for self-learning for the session and may not be required in near time - you can consider this as optional)**

* A lambda function is a small anonymous function.
* A lambda function can take any number of arguments, but can only have one expression.
* Syntax:

lambda arguments : expression

* Example:

![](https://lh3.googleusercontent.com/eg-W6Gu9K6pTxQ6qV\_t\_8YZUZ5dCE4k7Pl3kN0LiFamX3P-TU6WZlVCYbDBEORDgx4GXIQNFb07Y225R8HxSR\_OLS\_EJ\_XfxdICmFJQy8guKPv9EY6a9rR94YKfV-ty4HS0owfsjAXc)

### Python Lambda Function

A lambda function that adds 10 to the number passed in as an argument, and prints the result:

Here’s a short article about lambda function and its applications: [https://www.programiz.com/python-programming/anonymous-function](https://www.programiz.com/python-programming/anonymous-function)

### Python List Comprehension

* One of the Python’s most distinctive features is the list comprehension, which you can use to create powerful functionality within a single line of code.
* List comprehension is generally more compact and faster than normal functions and loops for creating list.
* MUST READ: Learn about list comprehension from here: [https://www.programiz.com/python-programming/list-comprehension](https://www.programiz.com/python-programming/list-comprehension)

### Python Regular Expression

* A regular expression is a special sequence of characters that helps you match or ﬁnd other strings or sets of strings, using a specialized syntax held in a pattern.
* Must Read: Go through the following link to get an overview of how regular expression are used in Python: [https://www.tutorialspoint.com/python/python\_reg\_expressions.htm](https://www.tutorialspoint.com/python/python\_reg\_expressions.htm)
* It is usually a confusing topic for most programmers. So don’t worry if you’re not able to fully understand it.
