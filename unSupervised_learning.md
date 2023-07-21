# KMeans Clustering and Scatter Plots

This repository contains Python code for KMeans clustering and scatter plots using the Iris dataset and the Seeds dataset.

## Prerequisites

- Python 3.x
- Pandas
- Matplotlib
- Scikit-learn

## Getting Started

1. Clone this repository to your local machine.

git clone <repository-url>

2. Install the required libraries by running the following command:

pip install pandas matplotlib scikit-learn

3. Run the Python script to perform KMeans clustering and generate scatter plots.

## Contents

1. `sepal_vs_petal.py`: Python script for performing KMeans clustering on the Iris dataset and generating scatter plots.

2. `Seed_Data.csv`: CSV file containing the Seeds dataset.

## Usage

### Iris Dataset

The `sepal_vs_petal.py` script performs KMeans clustering on the Iris dataset, plots sepal length vs petal length, and sepal width vs petal width, along with the cluster centroids.

To run the script:

python sepal_vs_petal.py

### Seeds Dataset

The `Seed_Data.csv` file contains the Seeds dataset. The script reads the dataset, performs KMeans clustering, and generates a scatter plot comparing 'A' vs 'LKG' features, along with cluster centroids.

To run the script:


python sepal_vs_petal.py


## Results

The script generates scatter plots for the Iris dataset (sepal length vs petal length and sepal width vs petal width) and the Seeds dataset ('A' vs 'LKG') with cluster assignments and cluster centroids marked in red.
