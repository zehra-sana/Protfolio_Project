# Matrix-Completion-Using-Random-Projection

In this paper, to solve matrix completion problem, we used Alternating Least Square Algorithm, as well as Random Projection to reduce the dimensionality of the matrix. 
For the matrix completion problem, we used a dataset consisting of three major components users,items, and ratings. This data is then transformed into a ratings matrix, with users as rows of matrix, items as columns and matrix elements as ratings. Several entries are missing inthe matrix because all users may not have rated all the items. These missing entries are denoted by ‘NaN’. This matrix is then transformed into a matrix of 0 and 1. There are several approaches to perform matrix completion.

In this paper, we have discussed matrix completion problem with various approaches such as Singular Value Decomposition (SVD) , Convex Optimization, Non-Negative Matrix
Factorization (NMF) and Alternating Least Square (ALS) . Firstly, matrix completion with SVD. It is used to decompose a matrix into two unitary matrices and a diagonal matrix. This method returns a matrix including some negative values. It is useful for determining the rankof a matrix, but it is relatively more expensive for larger datasets. Another approach, Convex Optimization is a mathematical optimization technique used in minimizing convex functions.
It works well for the matrix with low rank. This technique produces an appropriate matrix including negative values; however, the inclusion of random projection is significantly challenging for the data with higher dimensions. 

Next approach, NMF is nonnegative matrix factorization technique. It is a better approach for matrix completion problem as it returns an appropriate matrix with all non-negative entries. But the NMF does not have a tuning parameter to reduce the problem of overfitting.
Alternative Least Square is a matrix factorization technique that includes regularization parameter. The aim of ALS is to find two matrices users(U) and items(V ). It is a two-step process in which we fix user matrix U and find the optimal matrix V and other way round, we fix item matrix V and find the optimal matrix U. With this algorithm we implemented matrix completion that returns a matrix which is approximately equal to the original ratings matrix (user-item matrix), but to make the completed matrix more efficient, we reduceits dimensionality using random projection. 

Random projection is a simple yet effective dimensionality reduction approach that simplifies the complexity of high-dimensional data into lower dimensional spaces, preserving the original data. Motivated by the recent development of the Johnson-Lindestrauss lemma, we present a random projection type approximation with the Alternating least square algorithm for the matrix completion problem.
