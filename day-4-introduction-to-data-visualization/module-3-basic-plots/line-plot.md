# Line Plot

### What is Line Plot?

A line chart is used to represent data over a continuous time span. It is generally used to show trend of a variable over time. Data values are plotted as points that are connected using line segments.

### Creating a Line Plot (with 2 arguments)

* In Matplotlib we can create a line chart by calling the plot method.
* plot() is a versatile command, and can take an arbitrary number of arguments.

![](https://lh4.googleusercontent.com/5Kjct9rrbO4j-8vpIToRfD8jpLWfW9NYf9-gZ96XqVUyiW1vXdzhJoezjdw\_fizYGHNbE8M1FS3dt0lOEWacg9ATu7RdybQ-X4v2A6NkDMOV249ERSCvcAuIIx4Z-9bILhghWnZaBug=s0)

Because it is a line chart, matplotlib automatically draws a line to connect each pair of consecutive points that represent coordinates on the graph.

### **Creating a Line Plot (with a single argument)**

* We can make a graph with a simple line of code as mentioned in the image:

![](https://lh4.googleusercontent.com/rdaoWUCN-oEBALNsz4uKg6JiGwCoTxY5YdVhwvI8rSYgh72WGg-nq9FeduAJ3iGuEdy\_zNzmLU3C9k4StYgJplQE15PP-p06bzjw3BtIDyOhvQh-RDFiCZ5iS2bdD5-NzzCa3LX2h14=s0)

****

* You may be wondering why the x-axis ranges from 0-3 and the y-axis from 1-4.
* If you provide a list of n elements to the .plot() function, matplotlib will assume it is a sequence of  y  values, and automatically generates the  x  values for you as a range of n elements starting from 0.&#x20;
* Since python ranges start with 0, the default list x  has the same length as  y . Hence the  x  data will be \[0,1,2,3]. (Length same as y( 4) but starts from 0 instead)

### Applications of Line Plot

Using a line chart one can see the pattern of any dependent variable over time like share price, weather recordings (like temperature, precipitation or humidity), etc.&#x20;

Let's look at an example of the graphical representation of Netflix Paid Subscriber Count growth from 2012 to 2018:

![](https://lh3.googleusercontent.com/pemWcV4QIPh\_detYSwXpsrcXNc1oUv6iz2dCH2Pg21ACwmghh9JO0nWlQ81D\_QPzWtQv\_K\_-JeGuG3QRFvisJi6IMBRdvnsGFtSAOXLIPNGqTWVuZGGFvTDn6vU1\_hXSplHzgIcamxY=s0)
