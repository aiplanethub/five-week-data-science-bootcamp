# Series

### Learning Objectives

* What is Series?
* Create a Series

### Pandas Objects

Before we dive into series, let’s do a quick recap of pandas ‘objects’. At the core of the pandas library there are two fundamental data structures/objects:

* Series
* Data Frames

### What is Series?

* A one dimensional labeled array
* Can hold data of any type
* Are like a column in a table

### What can a Series have?

* A Series can have all the elements as numbers in it

![](https://lh5.googleusercontent.com/wO7QsugVe6WveW19Lh-3MwJw-LAj3LOuUXb7--B0V8kn\_7eftXtQ9efShIc11bFDSFmhQGZGFZhTb8ACBsSdI0On6baZy\_39h4uuKB8ic75zSEgIwhTwSlZpb9Amd15dAABvsYyC4WY=s0)

* A Series can have all the elements as strings in it

![](https://lh6.googleusercontent.com/ZHePfrOzeMJZoda-jkSbq2JLV4cKm65wK5nqLF3ibK6pS2BLKeap1yjmjFLnI-24G7WbSm79yEr09FrrwI\_\_d3fs-sqikB\_fWHkIWBMm1bljR3zIngmq\_-39PVqbEgXwVxDNKRNh6XA=s0)



* A Series can have its elements as both numbers and strings.&#x20;
* But the data type of the Series is always ‘object’ in this case

![](https://lh5.googleusercontent.com/uIqEeI5kk1werkquq42aBS1pLFmmn09KZ6MbDpXxRH0F5USlVEY-xroPA1xyTluURGri9AUx\_blS1oRrg5lXfPj65mSIRFWUjI6nBJTLh-\_IqCtoCiPpUmLheMo0HqcwnQgmRSPvFAU=s0)



* Series is like a list in Python which can take any type of value like integer, strings, float (or decimal value), etc
* All the items in series are labeled with indexes

![](https://lh6.googleusercontent.com/-cog8I5vTSgmz42KFjWa1pZa1v9ooH7W2aLf5-WLXAc3tWgMvR1XOOX4GlZBEn6elKfQv1n82H5HDUi8D9ALipu-BFRvfKqlQql5k\_FB6HFN0Z2vP-h\_oP8zPgIkYhdtPBwGdrUu9Ew=s0)

* **By default indexing starts from 0 in Series.**&#x20;

### **Human vs Python Index**

* Indexes that we (Human) understand

![](https://lh4.googleusercontent.com/s8Jl5Fqk79NPztvBhlrDOzYdi8CtK8vQ5I8GiDP4jI5qvHcxmV3M3VMg3wqogoJlafxm4bZDJPddhlPzG1DaMfHbAjatkNRUj7wBSPG-bNWQ87foeduJZZhMWLfd1mXJoT8-JlI1Mo8=s0)

* Indexes that Python Understand

![](https://lh3.googleusercontent.com/jmxuTB9yjDwpmFoortAI6a9ssLbrzAZkC05j8lp5735QcW8nvfL\_UsWPYDogKFq3tAOtfCEco00wIpmV5Ncsju0gqdztWp\_zDDa6vtq2HvDENZZ5sxCIbT8dZsVshRiBW-q4asIXxIY=s0)

**Well, it all starts with ‘0’. That’s the only difference.**

### **Create a Series**

*   Remember to import library before using it!

    **`import pandas as pd`**
* You can create your own Series using list

![](https://lh5.googleusercontent.com/6XrGlDXFU-53qYf8W51TFknPRREnzlwISbKm1plhAgPrJ6-mKM9rePs0F-Mf\_4Ju3rIrLootGFhmUdtwZCWXdA6h1c8fD1Ysc7RM1FMVHATi8V0cSp5ywG2QPhoAgxEbWund2kBJhYY=s0)

* You can create your own Series using a dictionary

![](https://lh4.googleusercontent.com/14zr2J0U1mk7KuVTkC7yE6mlNtgulE-MdZOhwlwQhWY5FhYiOKyc32DW5dIonSxsQ2n4j3Q2YyUr8nH2X\_cbxHFoHcAxBTvnNoT4jZiZlKnnCOPDvY2GartkCzcnOiji3CAoHkEtdjI=s0)
