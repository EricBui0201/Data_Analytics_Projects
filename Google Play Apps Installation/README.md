# Google Play Apps Installation Predictor
<img src="Images/img1.png" width="250">

### Objective
The Google Play Store data has enormous potential to drive app-making businesses to success. Actionable insights can be drawn for developers to work on and capture a big share of the Android market. Accordingly, I will build a multi-variate classification model to predict the total installations per app based on a set of features.

#### Problem Definition
The dataset used in this project is retreived from Kaggle, consisting of more than 10K unique apps with 11 features fetched from Google's Play Store.The biggest challenge is to transform my intial dataset into an optimized one through proper feature scaling and engineering and choosing the right fit model with the highest predictive power based on the following classification metrics:
- Accuracy
- Precision (Positive Predictive Value)
- Recall (True Positive Rate)
- F1-Score (Weighted Harmonic Mean of Precision and Recall)
- AUC-ROC (True Positive Rate vs False Positive Rate)

#### Tools Used
- Python
  - Libraries:
    - pandas
    - numpy
    - matplotlib
    - seaborn
    - sklearn.feature_selection
    - sklearn.cluster
    - sklearn.decomposition
    - sklearn.metrics
    - kmodes.kmodes
    - warnings
- Spyder
- Trello

#### Resources
- Kaggle - Google Play Store Apps
  - https://www.kaggle.com/lava18/google-play-store-apps
- Google Play Store Website
  - https://play.google.com/store
  
#### Process
- Data Acquisition
  - Kaggle Dataset: Google Play Store Apps
  - Shape of datasets: 10,841 rows, 13 columns
 
 <img align="left" src="Images/img_1.png" width="750">
 
- Data Cleaning
  - e.g. Data Type Correction, Uniformative or Repetitive Data, Duplicates, Null Values, Missing Data, Irregular Data (Outliers detection via plots & descriptive statistics)
  
  <img align="left" src="Images/img_2.png" width="1500">
  <img align="left" src="Images/img_4.png" width="1000">

- Data Transformation
  - Label Encoding - Ordinal Categorical Variable
  - Binning - Target Variable (5 Installation Brackets)
  - Grouping 
- Feature Scaling
  - Units transformation
  - Log Scaling
  
  <img src="Images/img_6.png" width="750">

- Checking Assumption 
  - Multicollinearity for Logistic Regression Model
- Feature Engineering
  - Filter Based
    - F-Classification
  - PCA
    - Dimensionality Reduction
  - Clustering
    - Kmeans
    - Agglomerative 
    - Kmodes
  - Evaluation
    - Silhoutte
    - Davies-Bouldin
    
   <img align="left" src="Images/img_7.png" width="350"><p>
   <img align="left" src="Images/img_8.png" width="500">
   <img align="left" src="Images/img_9.png" width="500">
   <img align="left" src="Images/img_11.png" width="1000">
   <img align="left" src="Images/img_12.png" width="1000">
   <img align="left" src="Images/img_13.png" width="1000">
   <img align="left" src="Images/img_18.png" width="1000">
   <img align="left" src="Images/img_19.png" width="1000">
   <img align="left" src="Images/img_20.png" width="1000">

    
- Modeling
  - Multivariate Logistic Regression
  - Multivariate Random Forest
- Analysis and Visualization
  - Descriptive and Predictive Analysis
  - Graphs 
    
   <img align="left" src="Images/img_14.png" width="1000">
   <img align="left" src="Images/img_15.png" width="1000">
   <img align="left" src="Images/img_16.png" width="1000">
   <img align="left" src="Images/img_17.png" width="1000">


