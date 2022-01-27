### Open the notebook and run the cells in sequential way

# TASK 1
## 

### Input: Feature model (Color Moments, Extended Local Binary Pattern, Histogram of Oriented Gradients), X (One of the 12 types), k (Number of desired latent semantics), Dimensionality reduction technique (Principal Component Analysis, Latent Dirichlet Allocation, Singular Valued Decomposition, K-means clustering).

### Output: Each latent semantic is presented in the form of a list of subject-weight pairs, ordered in decreasing order of weights and stored in a properly labeled output file. For example, when the main function of this task is given the parameters – CM, con, 4, kmeans, the file “T1-LS-CM-con-4-kmeans.txt” will be created.

# TASK 2
## Implement a program which, given a folder with images, extracts and stores feature descriptors for all the images in the folder.

### Input: Feature model (Color Moments, Extended Local Binary Pattern, Histogram of Oriented Gradients), Y (One of the 40 subjects), k (Number of desired latent semantics), Dimensionality reduction technique (Principal Component Analysis, Latent Dirichlet Allocation, Singular Valued Decomposition, K-means clustering).

### Output: A file containing top-k latent semantics of the images in the database. For example, when the main function of this task is given the parameters – HOG, noise02, 34, kmeans, the file “T2-LS-CM-3-23-PCA.txt” will be created.


# TASK 3
## Implement a program which, given a folder with images and an image ID, a model, and a value “k”, returns and visualizes the most similar k images based on the corresponding visual descriptors. For each match, also list the overall matching score.

### Input: Feature model (Color Moments, Extended Local Binary Pattern, Histogram of Oriented Gradients), k (Number of desired latent semantics), Dimensionality reduction technique (Principal Component Analysis, Latent Dirichlet Allocation, Singular Valued Decomposition, K-means clustering).

### Output: A file containing top-k latent semantics of the images in the database. For example, when the main function of this task is given the parameters – CM, 6, SVD, the file “T3-LS-CM-6-SVD.txt” will be created.


# TASK 4
## Implement a program which, given a folder with images and an image ID and a value “k”, returns and visualizes the most similar k images based on all corresponding visual descriptors. For each match, also list the overall matching score and the contributions of the individual visual models.
### TASK4 Final function:

### Input: Feature model (Color Moments, Extended Local Binary Pattern, Histogram of Oriented Gradients), k (Number of desired latent semantics), Dimensionality reduction technique (Principal Component Analysis, Latent Dirichlet Allocation, Singular Valued Decomposition, K-means clustering).

### Output: A file containing top-k latent semantics of the images in the database. For example, when the main function of this task is given the parameters – CM, 6, SVD, the file “T4-LS-HOG-5-SVD.txt” will be created.

# TASK 5
## Implement a program which, given the filename of a query image which may not be in the database and a latent semantics file, identifies and visualizes the most similar n images under the selected latent semantics.

### Input: Query image name (string), Feature model, Dimensionality reduction technique, Value of k, Value of n

### Output: Most similar n-images

# TASK 6
## Implement a program which, given the filename of a query image which may not be in the database and a latent semantics file, associates a type label (X) to the image under the selected latent semantics.

### Input: Query image name (string), Feature model, Dimensionality reduction technique, Value of k, Subject id Y

### Output: Most similar Types based on the distance

# TASK 7
## Implement a program which, given the filename of a query image which may not be in the database and a latent semantics file, associates a subject ID (Y ) to the image under the selected latent semantics.

### Input: Query image name (string), Feature model, Dimensionality reduction technique, Value of k, Type id X

### Output: Most similar Subjects based on the distance

# TASK 8
## Implement a program which (a) given a subject-subject similarity matrix, (b) a value n, and (c) a value m,
## – creates a similarity graph, G(V, E), where V corresponds to the subjects in the database and E contains node pairs vi, vj such that, for each subject vi, vj is one of the n most similar subjects in the database
## – identifies the most significant m subjects in the collection using ASCOS++ measure.

### Input: Transition Graph, n value, m value

### Output: Most significant m objects using the PageRank

# TASK 9
## Implement a program which (a) given a subject-subject similarity matrix, (b) a value n, ( c ) a value m, and three subject IDs
## – creates a similarity graph, G(V, E), where V corresponds to the subjects in the database and E contains node pairs vi, vj such that, for each subject vi, vj is one of the n most similar subjects in the database
## – identifies the most significant m subjects (relative to the input subjects) using personalized PageRank measure.

### Input: Transition Graph, n value, m value, 3 subject IDs

### Output: Most significant m objects using the PPR
