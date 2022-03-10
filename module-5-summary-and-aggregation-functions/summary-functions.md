# Summary Functions

### Learned Till Now

So far you have learned reading a data file, some methods to check the overview about data and selecting data from a dataframe.&#x20;

Those are not well enough information that we got about the data. A data scientist always want to understand the behaviour of data. For numerical columns we may want to know the mean value or median values of the data, the minimum value in the column and the maximum value in the column, etc. For categorical column we are interested to know things like the number of different categories in a column, the count of each category in a column, the maximum occurring category in a column, etc. Here we will look some of the techniques that will help you know the above information about your data.

### What is Summary?

* Summary is a term used for short version for a longer work
* Summary is a brief statement of the main points of something
* Confusing? Let’s understand through an example.

### Summary Functions

* Pandas has many simple "summary functions" (well, this is not an official name) that helps you to restructure your data in a very useful way and displays the useful information about the data
* Do you recall the **info()** method that we had used in the earlier module? This method has given us 6 to 7 main points about the data like number of observations and their range indices, name of columns with their data types and number of non - null entries in the particular column, etc.
* So **info()** is also a summary function/method
* Here we will see another summary function - **describe()**
* Import Pandas Library and load the dataset ‘exam\_scores.csv’

![](https://lh5.googleusercontent.com/M5I3smJ1T5JnUWjI9OA5tHOdrxzjBjzZEpuR0\_mMG61QswJmHJTVRPzfS3I\_wA9iwbiPcEj2cBwFlFR6n8Y0g2g0xicFuBCSRFfaBHcUqueAEzT47F4N5jFS-ja8GfXyHod6XVfoqsU=s0)

### describe( )

* describe() method by default returns the summary about the numerical columns only.&#x20;

![](https://lh5.googleusercontent.com/hubvgWJGU7EcTvm8D4O-T4IZn7jC4Z\_LpoXrPExZfndrWd3lFGVc3WZ5voTPE9eLQaDF1RFX\_beZZEWMBMp2WeWblzUblJ5pPOG3DMSz4AtnHdkRCwzxfkgqhQkoGiW339A8SngrNT8=s0)

* Don’t worry if you don’t know what does these terms in red box mean? You will know the meaning of these terms in further content.
* If we want to get summary about categorical column separately then we can use one parameter **'include'**.&#x20;

![Don’t worry if you don’t know what does these terms in red box mean? You will know the meaning of these terms in further slides](https://lh6.googleusercontent.com/2JXqGdLIKXWMrAASsPzuZiGf3kFVKqLBz\_cYJ6eoJUzeByE2qn6qTtT2YF6A-s0-kliEsBUAMmoi32plcXT3wRJNfcXqm6jvXLu\_jdxCIGnrYu9BtjnktgM\_yrE8qsWUopMa1ES7fPM=s0)

* The returned summary is all about the categorical columns.
* Also, we can get the summary about numerical and categorical column together using the same parameter **'include'**.

![Don’t worry if you don’t know what does these terms in red box mean? You will know the meaning of these terms in further slides](https://lh4.googleusercontent.com/inHEFJ8aaqOCYjM4mrOtfBPscYl1Tw4uEOnhgO1bdt61UnYX4YhpK2Nvpzooi4jTnGwIX4y2YyMMyucH0TfIzj2\_az12KMAlXM8jcOUVMpnZ-caktoG4WRMkPJSLFecLvNWCFhIBoJM=s0)

* We can see the above table includes the summary about both numerical and categorical column. A categorical column cannot have minimum or maximum values or mean and median. So the entries in these field for categorical column is 'NaN'.
* We had seen in previous module that this dataset has 5 categorical variables (gender, race/ethnicity, parental level of education, lunch and test preparation course) and 3 numerical ( i.e. integer) columns (math score, reading score and writing score).

![](https://lh6.googleusercontent.com/Q\_azdPqOuHSy6sSY7hy5nk1Qp3QhxdDXQV-fK1Ctdrjhd3qNTGRc8-T6mQR\_CwRKV7krpf4XD8U7wtWbB1ET5d0msRlR7WQpvR9LTyT2UdxqYiglvbii9BDF6TtyPAaPpMjnB2ccQtg=s0)

*   Let's see what information about the data is returned in the above table:

    * **count** - the count of non - null entries in the particular column. For example, gender column has 1000 non - null entries.
    * **unique** - the count of unique values in a column. Only for categorical column. For example, gender column has 2 unique values - male and female.
    * **top** - this is also for only categorical column. This tells which category is occurring maximum number of times. For example in gender column 'female' is occurring maximum number of times.
    * **freq** - this is again for categorical column only. This tells you the number of occurence of the category that is occurring maximum number of times in the column. For example, 'female' in gender column is occurring 502 times.
    * **mean** - the mean value of the numerical column. For example, the mean math score is 67.128
    * **std** - This is standard deviation of the numerical column. This tells you about the variation of data. Don't worry if you don't know about it.
    * **min** - the minimum value in the numerical column. For example, the minimum math score is 15.0
    * **25%** - the 25th percentile (or 1st quartile) value in the numerical column. For example, the 25th percentile value for math score is 58.0
    * **50%** - the 50th percentile (or 2nd quartile or the median) value in the numerical column. For example, the median math score is 67.0
    * **75%** - the 75th percentile (or 3rd quartile) value in the numerical column. For example, the 75th percentile value for math score is 78.0
    * **max** - the maximum value in the numerical column. For example, the maximum math score is 100.0
    * **NaN values** means for a particular column a particular summary value is not available. For example, for column gender ( a categorical column), do not have mean value or median value as these are the properties of numerical columns only.


* **We can also use describe() method on a particular column/series.**

![](https://lh3.googleusercontent.com/pfG3rUBuFNiLVY5MbORXLoUC70qnGtaBXs5twuxhjD\_uhgQsCBVXwklEU2oEuoo2daLd7kYctLpDP1CywtJJPiApxUMlIwfot60YE\_SUzPnMrAw8awrtgoZwdnUpGy5oUC0wA2mJHxI=s0)

* If the column name doesn't contain any space in it, you can use attribute style of selecting a column. For example we used attribute style of selection for 'gender' but not for 'math score' as it contains space.
* If you use attribute style of selection for ‘math score’, Python will throw an error.

![](https://lh5.googleusercontent.com/AjoEgZw7kEqls\_-9l4JLnRIXPdw5PWIA2X2kKJ5vYPH5t7fFFHg1t3Il7pSfKtFsE0EA-J93SUdLZrBM6Eg6Rohwf\_r7Zct5rKs7ZGU-XaxqQJO1NTDsQT9BPxHESH9fFCBCih\_4AH8=s0)
