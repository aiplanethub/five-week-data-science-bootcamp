# Reading & Write Files

### Learning Objectives

* Reading a data file
* Writing a data file

### Reading Data Files

* It is always good to be able to create a dataframe by hand. But, generally, we don’t create our own data by hand. We work on the data that already exists.
* Data exists in number of formats. The most basic of these is the **csv** file**. csv stands for comma-separated-value**

### **What is a CSV file?**

![](https://lh6.googleusercontent.com/DsagpckPHdq\_EQ6nkZf4Zym562keV2HuewT8yQPvP34tg7CgxByML3Ig62lNaW9Zr5npcYH9KpMVt-WcBGacOiUH09-bdDheQZE-noKSKv9QcelSBj5RYyAU36tQh7zuoASg1992GHo=s0)

* CSV files are normally created by programs that handle large amounts of data. They are a convenient way to export data from spreadsheets and databases as well as import or use it in other programs.&#x20;
* CSV (Comma Separated Values) is a simple file format used to store tabular data, such as a spreadsheet or database.&#x20;
* A CSV file stores tabular data (numbers and text) in plain text.&#x20;
* Each line of the file is a data record.&#x20;
* Each record consists of one or more fields, separated by commas.&#x20;
* The use of the comma as a field separator is the source of the name for this file format.

### How does CSV look like?

![](https://lh3.googleusercontent.com/TCWx7pDzHrrVy5H03MDv7RC5bTZgggArvczN450\_Nu8M4JprKjfGNpKB4OUoDCOIX6PoBmn8\_hKojRB1PpQ0RUOXjJ9wX3lUVyy8TnEi-Hm6rO9fHUcwzZWP4L\_5uunvaXuAChISohI=s0)

### Working with CSV files in Python

* For working CSV files in python, there is an inbuilt function named read\_csv.
* However, a common method for working with CSV files is using Pandas. It makes importing and analyzing data much easier.
* One crucial feature of Pandas is its ability to write and read Excel, CSV, and many other types of files.&#x20;

### Pandas read\_csv

* Functions like the Pandas read\_csv() method enable you to work with files effectively.&#x20;
* The read\_csv() function reads the CSV file into a DataFrame object.
* A CSV file is similar to a two-dimensional table and the DataFrame object represents two dimensional tabular view.
* The most basic way to read a csv file in Pandas:&#x20;

![](https://lh6.googleusercontent.com/uM90w5wy4EGaTDuk8Z-wsqvjo\_CoCFUD\_tUcROc2PA7KwKAgsFxnpjNE3DYhHBGMjP\_fR0X4xBNRPVwQ4IaKIRzWZYxEyMzWRz2N8w8ljg6tu2d1mj9ZwU4xumzaarTWt-pQ42OlZrw=s0)

* Now, let's understand how to provide filename

![](https://lh3.googleusercontent.com/VheY65y65D1h31Y1981RzJHvAINyuXybBX0GR\_9Bw0FjUrW40lDZZhC\_so3EwOh3apvsjDVgekSUpATSMs8ZMc6aovYAe1Oqi4dN25jcZKV8YOBJNP4XUGoY23HLxb8r\_EaqNmGSU1k=s0)

* There are many other things one can do through this function only to change the returned object completely.&#x20;
* For instance, one can read a csv file not only locally, but from a URL through read\_csv or one can choose what columns needed to export so that we don’t have to edit the array later.
* These modifications can be done by the various arguments it takes.
* We don’t need to memorise all the arguments though, let’s have a look at few important ones in the next two slides.

### Pandas to\_csv with example

* The easiest way to write DataFrames to CSV files is using the Pandas to\_csv function.
* **Syntax:**

![Where df is the name of your DataFrame](https://lh6.googleusercontent.com/VPq\_hvRUvZ32MFMOHrSaFSzcgk5HwT04nlO4cXOZv7vxLzOTQ8FJoS5KhwdEq9N1ab5qJY2vA-LOuAC70ObjNHx6BcgrcpRGzNSlsqa9KMZ83\_zl\_pXJ\_G0XFp90-IgTckbuAZoqbWg=s0)

* **If you want to export without the index, simply add index=False**

![](https://lh5.googleusercontent.com/dGyHByhKLu4qqopnbMZr9OU6jhUG9Uq0RG58j-lThZq4BJM5PFPCp5kBdN\_LvzTxTsEUPbA470tLU9mlRNEr26O89Z8YZhV-rwAIhd6uP1Zs8KsQccOx\_mtDhqLzjgbsKyAwFSyqRGw=s0)

* **Example:**

![](https://lh3.googleusercontent.com/X0TLenKvA7B11QFLdXrpdugpGtX8YLEmQW2tIKz3dvRvCV6uiIvKmJHlTjVWv2rN3jrdI\_NM7GZNhOsrbEu4-i7OpWyFgYQLGb\_nII3\_LOPPvHJPBT9hEHMLhbFPUxRSsGiPmhGgeYc=s0)
