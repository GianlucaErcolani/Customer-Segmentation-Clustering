# Customer Segmentation using Unsupervised Learning

The goal of this project is to segment a retail customer base into distinct groups using unsupervised machine learning algorithms in **R**. By analyzing purchasing behavior and income, the project aims to identify distinct customer personas to drive targeted marketing strategies.

### Project Structure

* `Customer_Segmentation.R`: Main R script containing the analytical workflow:
    * **Exploratory Data Analysis (EDA)**: Visualizing the statistical distributions of Age, Annual Income, and Spending Score using base R histograms and `ggplot2`.
    * **K-Means Clustering**: 
        * Using the **Elbow Method** (plotting Within-Cluster Sum of Squares - WSS) to determine the optimal number of clusters computationally.
        
        * Applying the K-Means algorithm (`k=5`, `nstart=25`) and visualizing the resulting customer segments and their centroids.
    * **Hierarchical Clustering**: 
        * Computing Euclidean distances and building agglomerative clustering models.
        * Comparing different linkage methods (Ward.D, Complete, Average, Single) through **Dendrograms** to validate the cluster structure.
        

### Dataset

The analysis is performed on a Mall Customers dataset containing the following key features:
* `Age`: Customer's age.
* `Annual Income (k$)`: Customer's annual income in thousands of dollars.
* `Spending Score (1-100)`: A score assigned by the mall based on customer behavior and spending nature.

### Results
Both K-Means and Hierarchical Clustering methods successfully converged on an optimal partition of **5 distinct customer segments** based on the relationship between their Annual Income and Spending Score.
