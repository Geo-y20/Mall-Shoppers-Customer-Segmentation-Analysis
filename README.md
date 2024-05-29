
# Mall Shoppers Customer Segmentation Analysis

This project aims to analyze the shopping behaviors and demographic profiles of customers visiting a mall using various clustering techniques. The insights gained from this analysis can help tailor marketing strategies, improve customer engagement, and enhance the shopping experience through targeted offers and services.

## Table of Contents

- [Dataset](#dataset)
- [Data Cleaning](#data-cleaning)
- [Data Transformation](#data-transformation)
- [Clustering Techniques](#clustering-techniques)
  - [K-means Clustering (Implemented from Scratch)](#k-means-clustering-implemented-from-scratch)
  - [K-means Clustering using Sklearn](#k-means-clustering-using-sklearn)
  - [K-medoids Clustering (Implemented from Scratch)](#k-medoids-clustering-implemented-from-scratch)
  - [Hierarchical Clustering](#hierarchical-clustering)
  - [Density-Based Clustering (DBSCAN)](#density-based-clustering-dbscan)
- [Results](#results)
- [Conclusion](#conclusion)
- [How to Run](#how-to-run)
- [Dependencies](#dependencies)
- [License](#license)

## Dataset

The Mall Shoppers Customer Segmentation dataset includes the following features:

- `CustomerID`: A unique identifier for each customer
- `Age`: Age of the customer
- `Gender`: Gender of the customer
- `Annual Income (k$)`: Annual income of the customer in thousands of dollars
- `Spending Score (1-100)`: A score assigned based on customer behavior and spending nature

## Data Cleaning

- Checked for null values and found none.
- Checked for duplicate values and found none.

## Data Transformation

- Applied Min-Max Scaling to standardize features to a range [0, 1].
- Applied Z-Scaling (Standardization) to standardize features to have a mean of 0 and a standard deviation of 1.

## Clustering Techniques

### K-means Clustering (Implemented from Scratch)

Implemented the K-means clustering algorithm from scratch, initializing centroids randomly, assigning clusters based on the nearest centroids, and updating centroids iteratively until convergence.

### K-means Clustering using Sklearn

Used the `KMeans` class from the `sklearn.cluster` module to apply K-means clustering and compared the results with the implemented version.

### K-medoids Clustering (Implemented from Scratch)

Implemented the K-medoids clustering algorithm from scratch, initializing medoids randomly, assigning clusters based on the nearest medoids, and updating medoids iteratively until convergence.

### Hierarchical Clustering

Performed agglomerative hierarchical clustering using Ward's method and visualized the results with a dendrogram.

### Density-Based Clustering (DBSCAN)

Applied DBSCAN to identify clusters based on density and effectively handled noise in the data.

## Results

The project identified distinct customer segments based on age, annual income, and spending score using various clustering techniques. The clustering results were visualized and analyzed to provide insights into customer behaviors.

## Conclusion

The analysis demonstrated the effectiveness of different clustering techniques in segmenting mall customers. These insights can be leveraged by businesses to develop targeted marketing strategies, personalize customer experiences, and improve overall customer satisfaction.

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/mall-shoppers-customer-segmentation.git
   cd mall-shoppers-customer-segmentation
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Mall_Shoppers_Analysis.ipynb
   ```

## Dependencies

- pandas
- numpy
- scikit-learn
- scipy
- matplotlib

Install the dependencies using:
```bash
pip install pandas numpy scikit-learn scipy matplotlib
```

