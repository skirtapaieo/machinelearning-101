# machinelearning-101

# 1 Math Concepts 

## Sparse Matrix Multiplication

### The question

Write a function that takes two integer matrices and multiplies them together. 

Both matrices will be sparse, meaning that most of their elements will be zero. 

Take advantage of that to reduce the  number of total computations that your function performs.

If the matrices can't be multiplied together, your function should return [[]]. 

<code>
matrix_a = [
    [0, 2, 0], 
    [0, -3, 5],
]
matrix_b =  [
   [0, 10, 0],
   [0, 0, 0],
   [0, 0, 4],
]
print(sparse_matrix_multiply(matrix_a, matrix_b))
</code>

### The solution 

See sparse-matrix-multiplication.py

### Why it matters? 

A sparse matrix is a matrix in which most of the elements are zero. 

The opposite of a sparse matrix is a dense matrix, where most of the elements are non-zero. 

Sparse matrices appear in many real-world situations, including:

- In social networks, where a matrix might represent connections between people. Most people are connected to only a small fraction of all other people, so the adjacency matrix is sparse.
- In text data, where a matrix might represent word frequencies in documents. Most words only appear in a small fraction of documents, so the document-term matrix is sparse.
- In scientific computing, when solving partial differential equations over a three-dimensional domain, the matrix that represents the domain is usually sparse.

Sparse matrices are important because storing and manipulating them in a naive way can be very inefficient. For example, if you store a sparse matrix as a standard two-dimensional array, you'll waste a lot of space storing zeros. 

Similarly, if you perform operations on a sparse matrix as though it were dense, you'll waste a lot of time multiplying by and adding zeros. This is why special data structures and algorithms for sparse matrices have been developed.

# 2 Model Concepts 

## K Nearest Neighbors


