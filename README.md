# Lower Back Pain Prediction Problem
## Project Overview
Lower back pain is a prevalent condition, often resulting from spinal misalignment and other biomechanical abnormalities. This project utilizes a dataset containing 12 potential indicators of spinal misalignment to identify clusters of patients with potential back pain issues. Since the dataset lacks a target variable, the analysis focuses on clustering techniques to uncover potential patterns.

## Key Objectives:
Explore feature distribution and identify key patterns in spinal metrics.

Apply Principal Component Analysis (PCA) to reduce dimensionality and capture major variance.

Implement K-Means clustering to identify patient groups based on spinal metrics.

Visualize clusters to intuitively distinguish between "normal" and "abnormal" cases.

## Dataset
The dataset includes 12 biomechanical features associated with spine alignment and potential causes of lower back pain.

## Key Features:

Pelvic Incidence, Pelvic Tilt, Lumbar Lordosis Angle, Sacral Slope, Pelvic Radius

Degree Spondylolisthesis, Pelvic Slope, Direct Tilt, Thoracic Slope, Cervical Tilt

Sacrum Angle, Scoliosis Slope

## Methodology
### Data Preprocessing:

Outlier Analysis: Outliers detected in Pelvic Tilt, Pelvic Radius, and Degree Spondylolisthesis were replaced by the median to minimize skew.

Feature Scaling: Standardized the dataset to ensure all features contribute equally to clustering.

### Exploratory Data Analysis (EDA):

Distribution Analysis: Visualized the distribution of each feature to identify patterns and outliers.

Correlation Matrix: Examined correlations to identify interdependent features.

### Principal Component Analysis (PCA):

Computed eigenvalues and eigenvectors to reduce dimensionality.

Selected 6 principal components explaining approximately 80% of the dataset variance.

### Clustering Analysis:

Applied K-Means Clustering with k=2, as suggested by the Elbow Method.

Visualized clusters to intuitively differentiate between normal and abnormal cases.

## Results & Findings
### Feature Distribution Analysis:

Significant outliers were identified in Pelvic Tilt, Pelvic Radius, and Degree Spondylolisthesis.

These features may potentially be key indicators of spinal abnormalities.

### Principal Component Analysis:

6 components were selected, capturing 80% of the data variance.

The first component exhibited the highest variance, indicating its potential influence on spinal alignment.

### Clustering Analysis:

The Elbow Method suggested k=2 as the optimal number of clusters.

Visualization of clusters indicates two distinct groups, which can be intuitively interpreted as normal and abnormal cases.

## Technologies Used
Python

NumPy, Pandas

Matplotlib, Seaborn

Scikit-Learn

Jupyter Notebook

