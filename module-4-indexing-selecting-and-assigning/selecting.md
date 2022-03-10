# Selecting

### Attribute(Dot) Based Selection

* We used shape attribute to know the shape of the dataframe. Do you recall this? If you don’t remember, follow the code below.

![](https://lh6.googleusercontent.com/\_QsqMDdCajh6t7B\_n9i0PEr86BzpDNJHQKct8DskwGCD3QOnhiFYTDCypcXijyfsz-QtILFfwceU\_ipD1d2hdOKhlDHld\_89cUFz5UzVDlkdS5TVcHZeJpmDGFqieNNlHbkZ0L1mC7s=s0)

* Similar to that, you can use a particular column name as an attribute to select a column.

### Dictionary(Bracket) Based Selection

* Do you recall getting a value from a dictionary using key? If you don’t remember, follow the code below.

![](https://lh3.googleusercontent.com/i1EQH4v1Gdtlgt9jODkmsCM0lwJ08\_xaUdfVuurZhKsd\_pWkXCirnmkqOmlq0jQL0Byoznc2ZieEsdt4TblXDA9ggOVERc0OFzIQQuqVwCIPAR8azuQFOOWz6Kf1Lumzk0RbcEobrnw=s0)

* Similarly you can use a column name to select a column from a dataframe. `df[column_name]`

### Selecting Multiple Columns

* While selecting multiple columns we use double square brackets \[\[]].

![](https://lh3.googleusercontent.com/UN-XFp9e8pedYV4ctGRNpIM46Lee5zXGasRFpEnqS\_P4bZ1-GS-RdJgnf56YlCFPUMF\_Jle-yeSAtfmiqLnkTG4jAKl5NUFrIbDmF3OTStVOtiKWQLmBlvXDJoUTBtnE-7LydThYKxs=s0)

### Conditional Selection

* Suppose you are interested to get data of ‘Jose’ from the given dataframe.&#x20;

![](https://lh5.googleusercontent.com/0bjUDhzCYycXMMlewiEFew244mrD-l9kI\_q\_rE9V9Hn6rBIUR6odYvqqJXHop7DG6c3S0pGxkGLgDNYNo8pnWmoS1DHpOuHB-NKZdM8KQTFj52d8oohhSmlCT0bbYejnwhChLeJmvzA=s0)

* We can make a condition using any conditional operators discussed in ‘Introduction to Python’ course. Let’s say we want the record where ‘Name’ is ‘Jose’. We can make condition here using == conditional operator\

* This will return a series of True/False values

![](https://lh4.googleusercontent.com/XknU0ySLXBtcJTmM-Ig\_t-78xQq1wdhV\_I0kl14ivmM6jd1fovFnkOrfyrNlVhTCo\_hk1zh37KPrs7cigZtGgJscqMThGEeypZKHGuMMUzUvWa\_IYplHhPZwubrdiiGDxf8ODnaSdnc=s0)

* Get all the columns of the row that satisfies the condition. Here the condition is to get the rows where Name is ‘Jose’

![](https://lh5.googleusercontent.com/ukfoeH\_rvIaKJ4P7KfpraWvddR3o2IgLjoPhfEf2UYXMPY2sLbeYinxPx7fJ5GxqlyO5VuCuoQS9u-lHRiWNxS6MuZDHi3GH8vyt2RA7VJgH1AfcsI7hAGz\_EKlZsbdbGoPxn9ns854=s0)
