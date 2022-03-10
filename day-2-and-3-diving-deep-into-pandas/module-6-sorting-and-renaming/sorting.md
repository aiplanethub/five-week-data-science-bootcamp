# Sorting

* Assume you are a teacher and you have scores of your students in the dataset ‘exam\_scores’ (say). You want to get the information about all the students whose performance is very bad in ‘math’.\

* What about going through all the records in the dataset and finding out manually the students whose score in math is very bad?\

* You can think of doing this manual task if you have 10 or 20 records. But here you have 1000 records. You need to figure out some easy way to do this. Here comes the importance of sorting technique.\

* The data present in the dataframe ‘exam\_scores’ is in the default index order not in a value order. \

* Pandas provides a method called sort\_values() which returns the sorted result in value order. \

* Let's say we want to get the student's information which are in increasing order of math scores.

![](https://lh6.googleusercontent.com/SOsZE-EdUqI4HGfyQkcWQXSVDnhsAtaECPSEHjmQOYwQf-\_u7USyM5gSpLBxUqUJrvQJWigNe0YzxWUiqxnMHJIA3J-uil1jV0gLM1J3CrU59Rh8PP851-UCxg2fhkyrkQsaWTTxAik=s0)

* By default the sorting happens in an ascending order.&#x20;

![](https://lh5.googleusercontent.com/DwsADR4seqRVyn\_NNRleMtrJuZSuAq9UgtqSWgpCpB8W-hjSkq5Gtpio7RuAzGXdaRsMtmETr\_TQHfRuwCX39Vns5x4wKxBFMwNQRZQzpFDpqF8v3ntbXkJ6\_yOQ4PwqzQ8wJSH9b4k=s0)

* We can get the sorted result in descending (decreasing) order by passing the parameter ‘ascending’ as False in the sort\_values() method.&#x20;

![](https://lh3.googleusercontent.com/-2HxdvhFSvxYEY1TQxWjHbeuE1gIvbAtD5C\_UlFaw0gg7jFM8I5c6IyFiKCXilIbEWid4xWGyHbjKy6CBIMR2whj9FgGzcXZWkm084hpm5avs-T6ohSWi22EKa7-ZkHq8CHEaMvR4hk=s0)

* We can also sort a series using the sort\_values() method.

![](https://lh4.googleusercontent.com/hA8w9r5LKnbZK6ablEfS9uHbCrzPzWBwfOTKInp7JI\_0PogfWvIlt27\_eFPI-GIv-JvPRDYSNlBu\_jUiRyho-3kMjrzsWl8xCImhV2npzPSTgtuCh3tu-F2PE\_3Ep0-tPNVKyzjsSYQ=s0)
