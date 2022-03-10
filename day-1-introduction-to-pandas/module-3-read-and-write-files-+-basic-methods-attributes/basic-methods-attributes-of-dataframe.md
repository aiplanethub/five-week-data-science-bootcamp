# Basic Methods/Attributes of Dataframe

## Dataset: **Exam Scores**

This dataset contains marks secured by different students in an examination and their background information.

The dataset can be found here:

* [https://github.com/dphi-official/Datasets/blob/master/exam\_scores.csv](https://github.com/dphi-official/Datasets/blob/master/exam\_scores.csv)

## Read The dataset

* So far you have learned how to read a csv file using read\_csv() function. Let’s see the practical implementation&#x20;
* read\_csv() function is of pandas library. So the first task is always to import/load the library we will use.

![](https://lh3.googleusercontent.com/Be5ivZsR1riNs5TejDCQ6P0dbDqnW1NveYYI0185tl1YIivBpmaR8QlctneE6lbnB8oAFbOu1AwfNY2VvxbEXBPXX2Iu-q4mcieDCb3W9dO9ROvY2Gs1aeFTan3U4eDzMV-0zUVa50g=s0)

* To read a csv file, use read\_csv() function of pandas library.

![](https://lh3.googleusercontent.com/HE0InvGdoZRT95wPdMPh3CPEA4TpJ8RjUmVHIcMGVEF76HmAq2yIOZEoRtpvhU0SwYQXQVudX75Z92VNp9XfrnaEf\_SmAqRe\_vFQa8SYYfZDdGrdR9-OKb08xuQldO8ikgP\_mOvqbLA=s0)

* **The csv file ‘exam\_scores’ is located in the current working direcroy**&#x20;

## **Methods/Attributes of Dataframe**

## **shape attribute**

* **shape:** It will help you to know what is the shape of your Dataframe i.e. (number of rows, number of columns)&#x20;
* After we have loaded the data we can check the shape of the Dataframe using shape attribute.

![](https://lh5.googleusercontent.com/JQKETs8xI5ew9lbgmBetB\_7coZXqD-pMtMljCwl-LWHg6C4f9wiukJzhzQohshvY5ld4oI0yotsFuB9nxowMmyFq5K0u12TGl7OIoqcDUStDHlSJx2KAnaXY\_G4vVghlYvzrJe6g23c=s0)

* So our DataFrame has 1000 rows and 8 columns. From here we can also say that our DataFrame has 8000 entries.

## **head( ) method**

* **head( ):** It will help you to see the first five observations of your dataframe. You can get some idea about the content of your dataframe.
* To get some idea about the content in the dataframe we can use head() or tail() method. Any one of the two can give us some idea about the content in the dataframe

![](https://lh6.googleusercontent.com/TTxLUzl4C1Q3D9nX\_rCJ8AEUfNs0ObIJ2\_K4OrUMj87FO2mhgr5X2REqmjvvqF53mL2dCTEYd1bijP6qPR3xErtPxyQBOcdp61lw1-\_fa88waODsSzI\_iyJ-LeaNDXIofF0iqhFF0ug=s0)

* **We can see the first five observation of the dataset in the above table.**&#x20;

## tail( ) method

* tail( ): This method is similar to head() method but instead of first five it will give you the last five observation from your dataset.

![](https://lh4.googleusercontent.com/9RqHr80vOxR5HyOx36bODVEDEYjBAnNsyH7Vyj34FMKAaVADOZFAKKI-aYjtBcoeCCtMdbeokEWdz0z6MM3Vqmh6v7XmXRChJkCx8uaYZ0GnvgH2\_g4x8082fEm-ZAlnEaMsJGwRAVQ=s0)

* **We can see the last five observation of the dataset in the above table.**

## **head( ) and tail( )**

We can also add the number of rows to be displayed in both head( ) and tail( ). See the example below:

![](https://lh3.googleusercontent.com/JDwD3GwrukYliNTysIoTn2Z0TU7yxVulWfeb3EE8Wkp68koXGifZhDPyVpfXhXczN-g65Y35S0zxeilRJnL2Dx3LTAkQ6OvaBK5sExUoaJ5Wp138pB2DOEm7aM9pRvDY7QVxfl2YVuE=s0)

## **dtypes**

* **dtypes** attribute: It will help you know about the data types of each column.
* To know the data types associated with each column, we can use dtypes attribute.

![](https://lh6.googleusercontent.com/yfqHtjHRX9Scz2WijVGY4oH8-VkA86nixuaxRwd\_CZaJ\_IKdHHvYVQOuOiY-b6u69LD5MwcSqsngoms1BhlJ-oU6mzrYkDhZR2hOs2cVjOiHtLn7WsMMZCZnVyMi1BtDORi1idyf\_Uw=s0)

We can observe here that the columns -

* 'gender', 'race/ethnicity', 'parental level of education', 'lunch' and 'test preparation course' are of data type - object.
* 'math score', 'reading score' and 'writing score' are of data type - int64 (i.e. integer)

## **info( )**

**info( )** method: This method will return you a concise summary about the dataframe.

![](https://lh3.googleusercontent.com/DV6WVYHkAefZm0\_Y1ymiJFv8nKxtn5IjzqIBui8qWWK5keLCilICBHOFCDrIqtC0ap0RmQkM-KD9nqasGMTi6MNZP\_BkeKuoSdol3Gl-f6cMk9PfHSu6frAHNQFI7w-npr8AxgZJt-o=s0)

**What you get using info() method?**

![](https://lh4.googleusercontent.com/4jkEtqfx1y4vBLI9lYDfkwER5IPvAdU6RowNVKf376E8b-WhA-FgNCG9TL4nUQ6ogWe1LT-RN3KEwhUOfm1KmDij9tMgWGRUrQrUxDyIMTiuQgzOOQPb3VoZs4c9yUL5cOWU5Jd\_18w=s0)
