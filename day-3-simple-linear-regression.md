# Day 3: Simple Linear Regression

### Learning Objectives

* Dependent and Independent Variables
* Equation of a Straight Line
* Linear Regression
* Cost

### Dependent and Independent Variables

* So far you’ve been studying input and output/target variables. Commonly, the input variable is known as independent variable and target variable is known as dependent variable.
* In nutshell, our target variable is nothing but a dependent variable. Why dependent? Because the values of this variable are dependent on other variables (i.e. input variables)
* And, our input variables are known as independent variables. Here the values of these variables are not dependent on any other variables.

Let’s look at some examples to learn more about them!

### Dependent and Independent Variables

* Remember the Standard Metropolitan Areas Data used in previous slides? In that dataset **we might be curious to predict “crime\_rate” in future**, so that becomes our target variable **(dependent variable)** and rest of the variables become input variables (**independent variables**) for building a machine learning model.

![](https://lh3.googleusercontent.com/BURnuNDFf72iHL6dGA4BfaoYllfFhmsIU-gxjyyqEWhdm6MMUkS3NM4SxNNWG5xtmBRZFPIw5Pnm5SavkmD8ZbqqplQSxT1J9cl3ow0UCgyiBXEBYDBR8hMPBHR-xZS8Ts08ksLfgUk)

### Another Example

* For example, a scientist wants to see if the brightness of light has any effect on a moth being attracted to the light.
* The brightness of the light is controlled by the scientist. This would be the independent variable.
* How the moth reacts to the different light levels (distance to light source) would be the dependent variable.

### Equation of a Straight Line

* In algebra, a linear equation (equation of a straight line) typically takes the form y = mx + b, where m and b are constants, **x is the independent variable, y is the dependent variable.**
* Basically, the value of y is being calculated using x whereas x has no dependence on value of y.
* y = how far up x = how far along m = Slope or Gradient (how steep the line is) b = value of y when x=0

![](https://lh6.googleusercontent.com/OaGsViGYz81XFJ4mHvNN6unULCfmtX1nDYqa3VlgU\_LJYvS9M8AiTEFD6q6YoXOw9m3eGO4Vh6wjKQzzVzAK9UTGG1KeHuE5mkDksxGiGxWpnZ31eaMgJETazxJ0nnKkin\_fsqcXHPQ)

* **How do you find "m" and "b"?**
  * b is easy: just see where the line crosses the Y axis.&#x20;
  * m (the Slope) needs some calculation:
  * ![](https://lh4.googleusercontent.com/jhEEyf0eV4qhw0B7dRsg2DMqbkDcw5WGVvjj-eWc\_-euBjhjEr0gjBnmVh8fO8sS2NknIOuUePqeiS425D4-ogRHT2cykG8BJRBgLsa-dZWRnPapBp7qKs0aidWx1JnQdgHFuckZYQo)

### Synonyms Recap

Too many synonyms to memorise? Let me put them all down at one place for better understanding:

* Variables = Features
* Input Variables = Attributes = Predictor = Independent Variables
* Target Variables = Labels = Outcomes = Dependent Variables

### What is linear regression? - an example

* Suppose you are thinking of selling your home. And, various houses around you with different sizes (area in sq.ft) around you have sold for different prices as listed below:

![](https://lh5.googleusercontent.com/BiM-JcHtH0vlUEZbFmv0SgfE5Q5q3nEZWoY86Zyc9gajS\_oryVx5XpD6yT1R62A-0iXyW5dGyIFrqKGZmeqHlKybmZIS4P\_pjCrAM7prTKNEZ06Hm2AYoddpvooZc9Zi10d3WGYZRJg)

* And considering, **your home is 3000 square feet**. How much should you sell it for?
* When you **look at the existing price patterns (data) and predict a price** **for your home** that is an example of **linear regression.**
* Here's an easy way to do it. Plotting the 3 data points (information about previous homes) we have so far:

![](https://lh3.googleusercontent.com/V2WsgQFVQvWaX8FFmAEss\_dyYj\_9S0kJdW3I3ZYmnq-DLnOLBugD7nkQWqZ2NO\_zr4bUwkd9B7JAVSrPk-kQAqgkCb7G8dQOw\_1ZcVEq9eu6NjSse0nB2zig9Bdkk3YjcDHH1-klYgE)

* Now you can eyeball it and roughly draw a line that gets pretty close to all of these points. Then look at the price shown by the line, where the square footage is 3000:

![](https://lh3.googleusercontent.com/V2WsgQFVQvWaX8FFmAEss\_dyYj\_9S0kJdW3I3ZYmnq-DLnOLBugD7nkQWqZ2NO\_zr4bUwkd9B7JAVSrPk-kQAqgkCb7G8dQOw\_1ZcVEq9eu6NjSse0nB2zig9Bdkk3YjcDHH1-klYgE)

* Boom! Your home should sell for $260,000.
* That's all! (Well kinda) You plot your data, make a rough line, and use the line to make predictions. You just need to make sure **your line fits** **the data well** (but not too well :)

![](https://lh3.googleusercontent.com/8bbBCXOPPTg2jwuI6hiEeUpMRoSNA4AqV5MbhruLijJYI8Gp\_Vd-XCXemfYSnIkdIAlmVCoASM4h6suu6P1y0PTcC2Vg4yU0D6laVOxSf7PheIoYyVlhxG33x6Mpje34m6K0TlIKx5Q)

**But of course we don't want to roughly make a line, we want to compute the exact line that best "fits" our data. That’s where**

### What is linear regression? - to summarize

* Linear regression is a linear model i.e. a model that assumes a **linear relationship** (straight-line relationship) between the input variables (x) and the single output variable (y).
* When there is a single input variable (x), the method is referred to as **simple linear regression** or just linear regression. **Eg:** Salary dataset given [here](https://github.com/dphi-official/Linear\_Regression\_Introduction/blob/master/Salary\_Data.csv). There is only one target variable and one input variable where we are predicting the salary of individual using their years of experience.
* When there are multiple input variables, it is often referred to as **multiple linear regression**. **Eg:** Smart Metropolitan areas data set, we have multiple input variables.

### Which line is good?

* **How do you decide what line is good? Here's a bad line:**

![](https://lh4.googleusercontent.com/uAt5GtGh4QUYu1srMGpETz1XrLOwdqGHBe1qVUdrmCfm3vPMMDzMxAKQegD6UTHJp69wIOxgo2K--wztRd0vHF3itSSP0aK\_t-gshsWCP8r1Nb\_IAYmugsvmElV5qe1IlViJ7jgyvEM)

* **This above drawn line is way oﬀ. For example, according to the line, a 1000 sq foot house should sell for $310,000, whereas we know it actually sold for $200,000.**

### **Here's a better line:**

![](https://lh3.googleusercontent.com/DRtyqH57Lga\_CN7YEhuF2cGJ4zmGizAhWaOQFrAhPY7rOGXwrLF8DsUvtRNSTCcH3JSuOUw0CVM65VqJbWjsOBVDKlI0qrpoNlnFgTH1Om5T9nDrJaFv7ldMkaws4oQ19Dpg5ugSXUQ)

* The **residual** (absolute diﬀerence between the actual and the predicted value) in this case are: $5000, $15000 and $5000.
* This line is an average of **$8,333** dollars oﬀ **** (adding all the distances and dividing by 3).
* This **$8,333** is called the **cost** of using this line.

### Cost

* The **cost** is how far oﬀ the **learned** line is from the **real data**. The best line is the one that is the least oﬀ from the real data.
* To find out what line is the best line (to find the values of coeﬃcients), we need to define and use a cost function.
* In ML, cost functions are used to estimate how badly models are performing.
* Put simply, a cost function is a measure of how wrong the model is in terms of its ability to estimate the relationship between X and y.

![](https://lh6.googleusercontent.com/scVcazKuVjxvMbIzy4HklgqANkZTQCgSUq0gcT4uft2A8MuS5vt\_pLQ\_xFZioR\_9R76kyo9jz1JGNjAceUrcgXBhAGMjtC9IkJjNFjw2vtSahYDNLFddR5FhhmR03nAzQhckAu-omO0)

### Cost Function

* There is also something called as Cost function that is associated with the analysis, it is slightly mathematical, we will be learning more about it soon!
* Meanwhile, let’s run a simple linear regression model using tf.keras. The link to notebook is given towards the end.

### Notebook for practice

* [https://dphi.tech/notebooks/892/manish\_kc\_06/introduction\_to\_linear\_regression? ](https://dphi.tech/notebooks/892/manish\_kc\_06/introduction\_to\_linear\_regression?)
