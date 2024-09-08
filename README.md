
---

# Socially Fair k-Means Clustering

This repository implements the **Socially Fair k-Means Clustering** algorithm, which focuses on reducing bias across sensitive attributes in clustering tasks. By considering fairness in optimization, this method aims to create more equitable cluster assignments across demographic groups while maintaining clustering performance.

## Overview

The Socially Fair k-Means Clustering algorithm addresses the issue of bias in traditional k-means clustering, particularly when sensitive attributes (such as gender, education level, and facial attributes) are present in the dataset. This project integrates fairness-aware optimization techniques, including Line Search and Gradient Descent, to mitigate bias while optimizing clustering performance.

### Features:
- **Bias Mitigation**: Incorporates sensitive attributes such as gender, education level, and facial features to reduce clustering bias.
- **Optimization**: Uses Line Search and Gradient Descent for fairness-aware clustering optimization.
- **Evaluation**: Plots clustering cost against the number of clusters, evaluating fairness by cost distribution across demographic groups.
- **Performance Metrics**: Achieved a silhouette score of 0.6 and near-equitable cost distribution across demographic groups.

## Datasets

This project utilizes the following datasets:
- **Adult Dataset**: Includes sensitive attributes like gender and education level.
- **UCI Credit Card Dataset**: Contains attributes related to credit card applications, including sensitive demographic data.
- **CelebA Dataset**: A large-scale face attributes dataset with sensitive attributes like gender, facial features, and other identity-related data.

## Clustering Performance

The performance of the Socially Fair k-Means Clustering algorithm is evaluated through:
- **Clustering Cost**: Visualized by plotting the clustering cost against the number of clusters.
- **Fairness Evaluation**: Near-equitable cost distribution is achieved across sensitive attributes like gender, education, and facial features.
- **Silhouette Score**: The final model achieved a silhouette score of 0.6, reflecting good clustering separation while maintaining fairness.
  **Fair K-means Clustering on Adult Dataset**
- https://colab.research.google.com/drive/1AlBp19kaSPfAk7PIomZVvNKWmVFLD5aG?usp=sharing

## Installation

To clone and run this project, use the following steps:

```bash
# Clone the repository
git clone https://github.com/your-username/Socially-Fair-k-Means-Clustering.git

# Navigate to the project directory
cd Socially-Fair-k-Means-Clustering

# Install the necessary dependencies
pip install -r requirements.txt
```

## Usage

After setting up the environment, you can run the following script to perform socially fair k-means clustering:

```bash
python main.py --dataset <dataset_name> --clusters <number_of_clusters>
```

### Arguments:
- `--dataset`: Choose between `adult`, `uci_credit_card`, or `celeba`.
- `--clusters`: Set the number of clusters for the k-means algorithm.

## Results

### Clustering Cost vs Number of Clusters:



![Average Clustering cost of different groups using Standard Lloyd](https://github.com/user-attachments/assets/73bb0875-b22d-4d1f-b584-24df927c3b0a)


Figure 1: Average Clustering cost of different groups using Standard Lloyd.

![Average Clustering cost of different groups using Fair Lloyd](https://github.com/user-attachments/assets/0114802a-2149-4e93-8936-c86423d5d657)


Figure 2: Average Clustering cost of different groups using Fair Lloyd.

### Clusters Determined by k-Means:

Below is a visual representation of the clusters determined by the k-means algorithm. The points are color-coded based on the clusters formed, indicating separation of data into distinct groups.


![3 means Clustering using FAMD](https://github.com/user-attachments/assets/95e5320c-5d07-4e77-b2bd-713666ba86e9)

Figure 3: 3 means Clustering using FAMD.

![5 means Clustering using FAMD](https://github.com/user-attachments/assets/59df595c-b031-4508-91e9-711bc41150b3)


Figure 4: 5 means Clustering using FAMD.


### Silhouette Score:

The silhouette score of **0.6** was achieved, indicating well-formed clusters with low overlap.

## Contributing

If you wish to contribute to this project, feel free to create a pull request or raise an issue.

# Made with :heart:
