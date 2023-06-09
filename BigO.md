# Big O: Analysis of Algorithm Efficiency

 Big O is used to describe the efficiency of an algorithm. This efficiency is evaluated based on :
 * time efficiency: The amount of time a function needs to complete.
 * space efficiency: The amount of memory resources a function uses to store data and instructions.

 To understand Big o as it should we must defind 4 topics 
1. Input Size
2. Units of Measurement
3. Orders of Growth
4. Best Case, Worst Case, and Average Case


### Input Size
Input Size refers to the size of the parameter values that are read by the algorithm. This does not simply refer to the number of parameters an algorithm reads, but takes into account the size of each parameter value as well. We will use the letter n to refer to the Input Size value. The higher this number, the more likely there will be an increase to Running Time and Memory Space.

### Units of Measurement
there is three Measurements of time:
1. The time in milliseconds from the start of a function execution until it ends.
2. The number of operations that are executed.
3. The number of “Basic Operations” that are executed.

there is four sources of Memory Usage during function run-time:
1. The amount of space needed to hold the code for the algorithm.
2. The amount of space needed to hold the input data
3. The amount of space needed for the output data.
4. The amount of space needed to hold working space during the calculation


### Orders of Growth
We can describe overall efficiency by using the input size n and measuring the overall Units of Space and Time required for the given input size n. As the value of n grows, the Order of Growth represents the increase in Running Time or Memory Space.

![Orders of Growth](LogPlot.png)

#####  O(1)
Constant Complexity means that no matter what inputs are thrown at our algorithm, it always uses the same amount of time or space. The number 1 is used to represent a constant value. The actual number of units will most likely be greater than 1, we round this number down to 1 to represent our estimate of complexity that is independant of n.

##### O(log n)
Logarithmic Time: The algorithm's runtime grows logarithmically with the input size. Examples include binary search or certain efficient algorithms on balanced trees.

##### O(n)
Linear Time: The algorithm's runtime grows linearly with the input size. Examples include iterating through an array or performing a simple linear search.
  
##### O(n log n) 
Linearithmic Time: The algorithm's runtime grows in proportion to the product of the input size and the logarithm of the input size. Examples include various efficient sorting algorithms like merge sort and quicksort.

##### O(n^2)
Quadratic Time: The algorithm's runtime grows exponentially with the input size. Examples include nested loops iterating over an array or performing a brute-force search.

##### O(2^n)
Exponential Time: The algorithm's runtime doubles with each increase in the input size. Examples include generating all subsets of a set or solving the traveling salesman problem using a brute-force approach.






### Worst Case, Best Case, Average Case
* Worst Case Big O : The efficiency for the worst possible input of size n
This case runs the longest for all possible inputs of n. This assumes that if we were sorting values, inputs are completely unsorted and searched values either don’t exist or are at the last to be searched.

* Best Case Big Omega: The efficiency for the best possible input of size n
This case runs the quickest for all possible inputs of n. In the case of sorting, this assumes that values are sorted, and so searched-for values are easy to find.

* Average Case Big Theta: The efficiency for a “typical” or “random” input of size n.
The average case makes a typical assumption about the possible inputs of size ‘n’ and how they might affect efficiency. This is NOT the best case and worst case averaged together.



