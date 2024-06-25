# K-Means and K-Medians Clustering

## Overview
This project involves implementing K-Means and K-Medians clustering algorithms from scratch. It explores the impact of different initialization strategies and distance metrics (Euclidean and Manhattan) on the clustering results and cost functions.

## Dataset
- `data.txt`: Contains the dataset with 4601 rows and 58 columns. Each row is a document represented as a 58-dimensional vector of features.
- `c1.txt`: Contains k initial cluster centroids chosen by selecting k = 10 random points from the input data.
- `c2.txt`: Contains initial cluster centroids chosen to be as far apart as possible using the Euclidean distance metric.

## Project Workflow
### 1. Exploring Initialization Strategies with Euclidean Distance
#### (a) Cost Function Computation
- Implemented K-Means clustering using Euclidean distance.
- Computed the cost function ϕ(i) for every iteration i.
- Ran K-Means on `data.txt` using `c1.txt` and `c2.txt`.
- Generated graphs plotting the cost function ϕ(i) as a function of iterations for both initializations.

#### (b) Percentage Change in Cost
- Calculated the percentage change in cost after 10 iterations for both initializations.
- Analyzed whether random initialization (`c1.txt`) is better than `c2.txt` in terms of cost reduction.

### 2. Exploring Initialization Strategies with Manhattan Distance
#### (a) Cost Function Computation
- Implemented K-Medians clustering using Manhattan distance.
- Computed the cost function ψ(i) for every iteration i.
- Ran K-Medians on `data.txt` using `c1.txt` and `c2.txt`.
- Generated graphs plotting the cost function ψ(i) as a function of iterations for both initializations.

#### (b) Percentage Change in Cost
- Calculated the percentage change in cost after 10 iterations for both initializations.
- Analyzed whether random initialization (`c1.txt`) is better than `c2.txt` in terms of cost reduction.

## Visualizations
Included in the Jupyter notebook are various visualizations such as:
- Cost function plots for both Euclidean and Manhattan distances.
- Comparison graphs for different initialization strategies.

## Dependencies
- Python
- Jupyter Notebook
- pandas
- numpy
- matplotlib
- pySpark
