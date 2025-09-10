# Provider Segmentation
### About
A complete data clustering internship project using __K-Means, Hierarchical Clustering, DBSCAN, Spectral Clustering, and Gaussian Mixture Model (GMM) Clustering__ to segment service providers into different groups based on selected features and also comparing each model's best possible performance.

<img src="https://tenor.com/en-GB/view/mitsuha-miyamizu-sayaka-natori-katsuhiko-teshigawara-your-name-kimi-no-na-wa-gif-25073719.gif" alt="みつは"/>
<hr>

### Key Principles
Data clustering is an __unsupervised machine learning technique__ that organizes and classifies different objects, data points, or observations into groups or clusters based on similarities or patterns. Unlike supervised learning, clustering does not rely on labeled data and instead aims to find natural groupings within the data.

Clustering is used to identify __underlying trends, patterns, and outliers__ in a dataset. It can be applied in various scenarios, such as exploratory data analysis, preprocessing, and anomaly detection. Clustering helps in reducing the complexity of large datasets by grouping similar data points together, which can simplify further analysis and visualization.
<hr>

## <b>Table of Contents</b>
**1st Phase - Exploratory Data Analysis (Data Cleaing & Transformation + Feature Engineering)**
* [Step 1 | Setup and Initialization](#setup)
    - [Step 1.1 | Importing Necessary Libraries](#libraries) 
    - [Step 1.2 | Loading the Dataset](#load_dataset)
    - [Step 1.3 | Dataset Description](#data_description)
* [Step 2 | Exploratory Data Analysis](#exploratory_analysis) 
    - [Step 2.1 | Dataset Overview](#overview) 
    - [Step 2.2 | Summary Statistics](#statistics)
    - [Step 2.3 | Data Visualization](#visualizations)
        - [Univariate Analysis (Single Variable)](#univariate)
        - [Bivariate Analysis (Two Variable)](#bivariate)   
        - [Time-based Analysis](#time-based)
* [Step 3 | Data Cleaning & Transformation](#data_cleaning)
    - [Step 3.1 | Handling Missing Values](#missing_values)
    - [Step 3.2 | Handling Duplicates](#duplicates)
    - [Step 3.3 | Treating Cancelled Bookings](#cancelled_cleaning)
    - [Step 3.4 | Correcting Date Anomalies](#date_cleaning)
    - [Step 3.5 | Ensuring Data Consistency](#data_consistency)
        - [Same-day Inconsistency](#sameday_inconsistency)
        - [Status Inconsistency](#status_inconsistency)
        - [Geographic Inconsistency](#geographic_inconsistency)
        - [IDs Inconsistency](#id_inconsistency)
    - [Step 3.6 | Outlier Treatment](#outlier_cleaning)
* [Step 4 | Feature Engineering](#feature_engineering)
    - [Step 4.1 | RFM Features](#rfm_features)
        - [Step 4.1.1 | Recency (R)](#recency) 
        - [Step 4.1.2 | Frequency (F)](#frequency)
        - [Step 4.1.3 | Monetary (M)](#monetary)
    - [Step 4.2 | Service Type Diversity](#type_diversity)
    - [Step 4.3 | Behavioral Features](#behavioral_features)
    - [Step 4.4 | Cancellation Insights](#cancellation_insights) 
    - [Step 4.5 | Seasonality & Trends](#seasonality_trends) 
    - [Step 4.6 | Advanced Provider Features](#advanced_features) 
    - [Step 4.7 | Export Feature Engineer Data](#export_features) 
        - [Provider Dataset Description](#provider_description)
* [Step 5 | Data Preparation for Clustering Models](#data_preparation)


## <b>Clustering Pipeline</b>
**2nd Phase - Data Modeling & Analysis**
* [Step 1 | Config](#config) 
* [Step 2 | Setup](#setup)  
* [Step 3 | Data Load (mock with numeric + categorical, or external)](#data_load)
    - [Step 3.1 | Dataset Description](#data_description)
* [Step 4 | Feature Mapping (with optional one-hot encoding)](#feature_mapping)
* [Step 5 | EDA](#eda)  
    - [Step 5.1 | Feature Visualization](#feature_visualization)
* [Step 6 | Missing Values & Casting](#missing_values)
    - [Imputation Methods Theory](#imputation_theory)
* [Step 7 | Feature Engineering](#feature_engineering)  
* [Step 8 | Feature Selection](#feature_selection)  
* [Step 9 | Outlier Handling](#outlier_handling)  
    - [Outlier Handling Theory](#outlier_theory)
* [Step 10 | Scaling](#scaling)  
    - [Step 10.1 | Compare Clustering Across Two Scalers](#compare_scalers)
* [Step 11 | PCA](#pca)
    - [Principal Component Analysis Theory](#pca_theory)
    - [Step 11.1 | 3D PCA Visualization](#pca_visualization)  
* [Step 12 | Clustering Models](#clustering_models)  
* [Step 13 | Hyperparameter Sweeps](#hyperparameter_sweeps)  
* [Step 14 | Validation Metrics](#validation_metrics)  
    - [Validation Metrics Theory](#validation_theory)
* [Step 15 | Visualization (scatter + centroids)](#visualization)  
* [Step 16 | Cluster Profiling](#cluster)
    - [Step 16.1 | Cluster Characteristic visualization](#cluster_characteristic)  
    - [Step 16.2 | Cluster Naming (business interpretation)](#cluster_naming)
* [Step 17 | Export artifacts](#export_artifacts)  
    - [Export Artifacts Theory](#export_theory)
<hr>

### Main Process
- Exploratory Data Analysis (EDA)
- Data Preprocessing (Data Cleaning & Transformation)
- Feature Engineering (Feature Extraction & Selection)
- Data Preparation
- K-Means Clustering
- Hierarchical Clustering
- DBSCAN
- Spectral Clustering
- Gaussian Mixture Model Clustering
- Silhouette Score
- Davies-Bouldin Index
- Calinski-Harabasz Index
<hr>

### Getting Started
This project contains two Jupyter Notebooks that document the **process** and **results** of the internship work.  
Since the dataset may be confidential, it is **not included** in this repository.

- `provider_segmentation_eda.ipynb` – Exploratory Data Analysis (EDA) of provider-related data.  
- `provider_segmentation_clustering.ipynb` – Clustering process and resulting segmentation.

You can open these notebooks in Jupyter Notebook, JupyterLab, or Google Colab to review the workflow and outputs.
<hr>

### License
This project is licensed under the Apache-2.0 License - see the LICENSE file for details.
