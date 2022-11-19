# unsupervised-machine-laerning-challenge

In this challenge I was part of data science team of a medical research company that’s interested in finding better ways to predict myopia, or nearsightedness. My team has tried—and failed—to improve their classification model when training on the whole dataset. However, they believe that there might be distinct groups of patients that would be better to analyze separately. So, my supervisor has asked me to explore this possibility by using unsupervised learning.

I was provided with raw data, so first I need to process it to fit the machine learning models. Then I usedseveral clustering algorithms to explore whether the patients can be placed into distinct groups. Finally, I was tasked with creating a visualization to share my findings with my team and other key stakeholders.

Part 1: Prepare the Data
Read myopia.csv into a Pandas DataFrame.
Remove the "MYOPIC" column from the dataset.

Note: The target column is needed for supervised machine learning, but it will make an unsupervised model biased. 
Standardize your dataset so that columns that contain larger values do not influence the outcome more than columns with smaller values.

Part 2: Apply Dimensionality Reduction
Perform dimensionality reduction with PCA. How did the number of the features change?
Using PCA(n_components=0.99) creates a model that will preserve approximately 99% of the explained variance, whether that means reducing the dataset to 80 principal components or 3. For this assignment, preserve 90% of the explained variance in dimensionality reduction.
Further reduce the dataset dimensions with t-SNE and visually inspect the results. To do this, run t-SNE on the principal components, which is the output of the PCA transformation.

Create a scatter plot of the t-SNE output. Are there distinct clusters?

Part 3: Perform a Cluster Analysis with K-means
Create an elbow plot to identify the best number of clusters. Make sure to do the following:

Use a for loop to determine the inertia for each k between 1 through 10.

If possible, determine where the elbow of the plot is, and at which value of k it appears.

Part 4: Make a Recommendation
Based on your findings, write up a brief (one or two sentences) recommendation for your supervisor in your Jupyter Notebook
