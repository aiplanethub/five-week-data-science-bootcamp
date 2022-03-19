# Linear Algebra

### Learning Objectives

* Linear Algebra
* Matrix
* Basic Statistics

### **What is Linear Algebra ?**

* Often the ﬁrst acquaintance with linear algebra looks something like this:

![](https://lh3.googleusercontent.com/sKgF5MgsTODk1WvPWVppCui19DUgZwwA3y4tx0RwkLe1IgxF54e4Frl\_dh7\_qFWNdutpcLOYr5hEMp1m\_leShY1iYhpoxTM9MjJA\_wETlLNrt7xrFHh9g7IFXta6yi3ugO63Av\_UPiw)

* Not very inspiring, right? Two questions immediately arise: where did all this come from and why is it needed.
* **Basic definition: Linear algebra is a sub-ﬁeld of mathematics concerned with vectors, matrices, and linear transforms.**

### Do we really need Linear Algebra ?

* It depends on your goal.
* If you just want to use tools from AI and machine learning as a black box, you arguably just need enough math to ﬁgure out if your problem ﬁts the models premise.
* But, if you want to develop new ideas, Linear Algebra is your must-learn thing. I don’t mean you need to learn everything concerning math. Doing so you will be stuck at everything and lose motivation towards other more important things like calculus/stats.
* Mathematics in data science and machine learning is not about crunching numbers, but about what is happening, why it’s happening, and how we can play around with diﬀerent things to obtain the results we want.

### Linear Algebra

* Let’s start with a simple problem.
  * Condition 1: Imagine price of 2 chocolates and 1 apple is 100 units
  * Condition 2: Similarly imagine, price of 1 chocolate and 2 apples is 100 units.

#### Now, we want to ﬁnd the price of a chocolate and an apple

* Suppose the price of a chocolate is $ ‘x’ and the price of an apple is $ ‘y’. Values of ‘x’ and ‘y’ can be anything depending on the situation i.e. ‘x’ and ‘y’ are variables.
* Translating the above information in mathematical form:&#x20;
  * 2x + y = 100 ---------- (1)
  * Similarly, for the second condition: x + 2y = 100 ---------- (2)
* To ﬁnd the prices of chocolate and apple, we need the values of ‘x’ and ‘y’ such that it satisﬁes both the equations.
* The basic problem of linear algebra is to ﬁnd these values of ‘x’ and ‘y’ which is nothing but solution of set of linear equation.

### Graphical Representation of two Equations

![](https://lh4.googleusercontent.com/Cjv10nggaVgHevwJ1odCIptKTKs2hHzlRbCPd\_POkFitFKz6vZ7NG7zLYt0KrSzbLC-p-jrEKUYTuPeCMXuq2HS8neIr5SJfZvoXNp0EfgS5mhSuDHy5Oo0Cis7HEQB9cn3G3CLYj6c)

* The intersection point is the solution of these two equations

### Complicating the Problem

* In the earlier example, we had two variables ‘x’ representing the price of a chocolate and ‘y’ representing the price of a apple.
* Now, suppose you are given a set of three conditions with three variables, say ‘x’, ‘y’ and ‘z’, and asked to ﬁnd the value of three variables.
* The three conditions are given as:&#x20;

x + y + z = 1 ---------- (1)

2x + y = 1 ---------- (2)

5x + 3y + 2z = 4 ---------- (3)

* By solving the above three equations we can get the values for ‘x’, ‘y’ and ‘z’.
* In Linear Algebra, data is represented in the form of linear equations. These linear equations are in turn represented in the form of matrices and vectors.

### Matrices

* Matrix is a form of **representing data in the form of rows and columns.** It is a very natural approach of organizing data.
* A real life example, consider a reactor which needs to be controlled using multiple attributes from various sensors like Pressure (P), Temperature (T), Density (d), etc.
* In the matrix given,&#x20;

&#x20;    P       T          d

![](https://lh3.googleusercontent.com/6JxR8xaFL0c1VSoAjASqHeteq3UEQSryfUycoks0BoCvycP-f4JRV60pkWXJDLjTkorsqWWAH1IVqCAKi0K5B-E\_Jp24wEb\_EjI6Cc2expmZIbU7zxQUo2JrFamO\_2JXetWTm9ImqbE)

* Columns:
  * First column represents Pressure (P)
  * Second column represents Temperature (T)
  * Third column represent Density (d)\

* Row: Each row corresponds to one sample.
* The image stored in the machine is nothing but a large matrix of pixel values across the image.

![](https://lh6.googleusercontent.com/Hns6w5a5GPPy3tR9VuL3u5i1r9m7TTuVcqn9W57YorNXAF-itsnRimAVfKIIsahEyLGEEHnPK9vP0iF6HjuigCs2VDSNwYM0y8poVDlTRlURXAJw9B0Rqkn1ofVQ3FU-zphrHTUBjes)

### Linear Equations in Matrix Form

* Earlier we had two linear equations as:

2x + y = 100 ---------- (1), and

x + 2y = 100 ---------- (2)

* The above two linear equations can be represented in the matrix form as:

![image](https://user-images.githubusercontent.com/51357266/158958132-9114ae70-45cc-4ace-af0f-75f6d6efe4a1.png)

* We can get the above two linear equations from the shown matrix equation just by multiplying the two matrices on left hand side and equating the corresponding value to right hand side.
* **Here is nice resource on Matrices for further reading:** [https://www.statisticshowto.com/matrices-and-matrix-algebra/](https://www.statisticshowto.com/matrices-and-matrix-algebra/)
