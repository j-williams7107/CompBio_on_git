#Lab 07: Writing Your Own Functions

		# step 1:
		
		# step 2:
		
		return(results)

1 , 1 , 2 , 3 , 5 , 8 , 13 , 21 , 34 , 55 , 89 , 144 , ...   
Often, especially in modern usage, the sequence is extended by one more initial term:  0 , 1 , 1 , 2 , 3 , 5 , 8 , 13 , 21 , 34 , 55 , 89 , 144 , ...  
By definition, the first two numbers in the Fibonacci sequence are either 1 and 1, or 0 and 1, depending on the chosen starting point of the sequence, and each subsequent number is the sum of the previous two.






Write a function that implements this model.  The function should do the following:

a. Take parameters as arguments (inputs).  This includes the following as parameters: initial population size (`n[1]`), total number of generations, `r`, `K`.
c. iterate the model
d. make a plot with axes properly labeled.
e. return the abundance data.

#####Problem #3
Social networks are very much "in vogue" these days, being used in many fields to understand all sorts of problems, from the transmission of disease to the spread of memes.  There are two very common ways that simple network data can be represented.  

(a) An "adjacency matrix": 	Suppose there are `n` individuals.  Then a matrix with `n` rows and `n` columns can be constructed.  The entry in the matrix at position `[i,j]` (i.e., the ith row and jth column) is zero if there is no interaction between individuals i and j.  If those two individuals do interact then the entry at position `[i,j]` is a number representing the strength or nature of the interaction.  In a very simple matrix, it could just be a "1" if there is an interaction of any kind, and a zero other wise.

(b) A table listing all non-zero pairwise interactions.  This is an `m x 3` matrix (`m` rows and 3 columns) in which the first column is the index or ID of a "row" individual, the second column is the index or ID of a "column" individual, and the third column is the number that represents the strength/nature of the interaction between these two individuals.

Write **two** functions.  The first function should take a square matrix of any size and turn it's contents into the pairwise table form.  The second function should do the reverse (i.e., take a pairwise interaction table and turn it into a square matrix).  **The first function is required.  The second function is a bonus problem.**

Examples:

Function #1 should take this:

| 0 | 1 | 1 |  
|  
| 1 | 0 | 0 |  
| 1 | 0 | 0 |  

And turn it into this:  

|row|column|value|
|
|1|2|1|
|1|3|1|
|2|1|1|
|3|1|1|

Function #2 should do the reverse.  Note that the list form only includes the non-zero entries of the matrix.
 
If you want to test that your functions work, import the data given in the Lab07 folder in the file called "SmallAdjacencyMatrix.csv".  Try converting those data with the first funcion.  Then, if the results look fine, try to recreate the SmallAdajcencyMatrix by using your second fuunction on the . 