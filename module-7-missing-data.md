# Module 7: Missing Data

### What is a Missing Value?

* If in any row or column in a dataframe, the value is not available, it is said as the missing value.\

* So defining missing data: **Missing data (or missing values) is defined as the data value that are not stored in a column or row.**\
  ****
* Consider this small dataset which has some missing values in it (shown in the red box).

![](https://lh4.googleusercontent.com/cV1tAA3TXSS975NmnbJm4pbEeud1-YF2K4ATYv59dVu4OCCMRADcNA8zHr5-Qxf6F8VhswiSOafAmKnM7U1CCqSISwN35N\_QM3cpC-9k\_gQeGUOYaZYSC4-hG3XgrHQ5LMu0bpwotzA=s0)

* Well this is a small dataset so we can easily observe the missing values here. But real data are very large in size and you cannot easily see the missing values in the dataframe.\
  &#x20;
* Pandas provides **isnull(), isna()** functions to detect missing values. Both of them do the same thing.\

* **df.isna() or df.isnull()** returns the dataframe with boolean values indicating missing values.

![](<.gitbook/assets/Screen Shot 2021-09-25 at 5.45.32 PM.png>)

* We can get column wise count of all the missing values using the aggregation function **sum()**

![](https://lh4.googleusercontent.com/fQ2iF15TDtteBT8yFgCiR1mW0b2LhplXFDbZYk3Q1YuZkOlfB31KzRPgfW4ViWSiyuYP1uOJKM9Gr5Y9X8H7JQoWw39C2nABc7SJf\_1xcrJoo8FiyywmoeoBuqC3RsnoxbrBLUGgwsM=s0)



* Both the columns 'Names' and 'Marks%' have one missing values in each. 'Regd. No' has no missing values so the value is 0.\

* Pandas also provides fillna() method to fill the missing values. fillna() provides many different strategy to fill the missing values.\

* Let's say we want to fill the missing values in 'Names' column with 'unknown'.

![](https://lh4.googleusercontent.com/fgFoN\_VNl3LPnlcG8nzg3ZYWoIbCSIjSN6fP1DZFv16Nk6WmlSjDqt0OWFdFt1-rS4LQqSLHLbE-E3ht-UdOmWYchZYc7HEa9rz1bxpdVT-ErTOg7\_4jpv3SZfUNeUPJaXW\_vGUx5y0=s0)

* But the changes are not made inplace.\

* The dataframe still contains missing values in the 'Names' column.

![](https://lh3.googleusercontent.com/h9xvaygv9OkETQd6UTFeQoBzc9kuDqe4xc36GTobuAsU1M40qx5kW98iGM-bhG5h75w\_sPt141X2dYM88ofVCx4vn8bT5LJGdlf0h-PduLnzXF24qowrjygLDf-CTLumV-WDrYSZAZ0=s0)

* We can pass 'inplace' parameter as True in fillna() method. It will make the changes in the original dataframe.

![](<.gitbook/assets/Screen Shot 2021-09-25 at 5.48.32 PM.png>)

* There is still a missing value in 'Marks%' column. Let's say we want to fill the missing value in this column with the mean of the marks scored by other people.

![](https://lh6.googleusercontent.com/bJY0UFo7JSCOSXqjj6eVA2LYqyqPgmyCUAqXjzi6FZ64krbmPsgCutAgz12kgtJnLy7bjwB2cS6SdBuGuP9FzZf\_gyEk\_jpYH64Mjbw6L9kv9-AkbPhHU0eF8Z675ZfRj\_gKU1lFeBM=s0)

* Now, our dataframe has no missing values.
