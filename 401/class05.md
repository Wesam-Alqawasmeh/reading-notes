# Linked Lists

-----


## Big O: Analysis of Algorithm Efficiency

**Overview**

- the role of Big O in algorithm efficiency is to describe the Worst Case of efficiency an algorithm can have in performing it’s job.

- TO evaluate Big O you need tow factors which are:

1. Running Time (time efficiency / complexity): it is the amount of time a function needs to complete.

2. Memory Space (space efficiency / complexity): it is the amount of memory resources a function uses to store data and instructions.

**To analyze Big O factors we need we should consider 4 keys**

**1. Input Size**

- refers to the size of the parameter values that are read by the algorithm. This does not simply refer to the number of parameters an algorithm reads, but takes into account the size of each parameter value as well.

- The higher the input size value get, the more likely there will be an increase to Running Time and Memory Space.

![On](https://miro.medium.com/max/742/1*WBYUz6Lh2Z21DQnEk-MWFQ.png)

![notation](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQmycL50k7v9h80C05_SjEh0-gDKDDfuQ6RtQ&usqp=CAU)

**2. Units of Measurement**

- In order to quantify the Running Time in our analysis, we will consider Three Measurements of time:

 1. The time in milliseconds from the start of a function execution until it ends.

 2. The number of operations that are executed.

 3. The number of “Basic Operations” that are executed.

 

 - In order to quantify Memory Space, we can consider Four Sources of Memory Usage during function run-time:

 1. The amount of space needed to hold the code for the algorithm.

2. The amount of space needed to hold the input data.

3. The amount of space needed for the output data.

4. The amount of space needed to hold working space during the calculation.

**3. Orders of Growth**

- We can describe overall efficiency by using the input size n and measuring the overall Units of Space and Time required for the given input size n. As the value of n grows, the Order of Growth represents the increase in Running Time or Memory Space.


**4. Worst Case, Best Case, Average Case**


- Worst Case: The efficiency for the worst possible input of size n

- Best Case: The efficiency for the best possible input of size n

- Average Case: The efficiency for a “typical” or “random” input of size n



