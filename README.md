# breast-cancer-classification-ml
Breast cancer is a common and life-threatening disease. This project applies machine learning models to classify tumors as benign or malignant based on cell features and identify the most accurate model.
Breast Cancer Classification Using Machine Learning

A machine learning project focused on analyzing medical data and building classification models to predict whether a breast tumor is benign or malignant.

The project follows an end-to-end machine learning workflow, including data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and comparison across datasets.

Project Overview

The project uses the Breast Cancer Wisconsin Diagnostic Dataset, which contains numerical measurements describing characteristics of tumor cells.

The main objective is to develop classification models that can distinguish between benign and malignant tumors and evaluate their performance using multiple classification metrics.

A secondary experiment uses the Iris dataset, converted into a binary classification problem, to compare model behavior across different datasets.

Dataset

Breast Cancer Wisconsin Diagnostic Dataset

* Records: 560
* Features: 30+ numerical features
* Target: diagnosis
* Classes:
    * 0 — Benign
    * 1 — Malignant
* Source: Kaggle (CSV)

The dataset contains measurements such as:

* radius_mean
* texture_mean
* perimeter_mean
* area_mean
* smoothness_mean
* compactness_mean

Unnecessary columns were removed, and the dataset was checked for missing values.

Technologies & Tools

* Python
* Pandas
* NumPy
* Scikit-learn
* TensorFlow / Keras
* Matplotlib
* Seaborn
* Jupyter Notebook

Project Workflow

1. Data Preprocessing

The preprocessing stage included:

* Removing unnecessary columns
* Checking for missing values
* Encoding the target variable
* Splitting the data into training and testing sets
* Feature scaling where required

The dataset was divided into:

* 70% Training
* 30% Testing

A fixed random state of 42 was used to support reproducibility.

2. Exploratory Data Analysis

Several exploratory analyses were performed to understand the dataset and identify meaningful patterns.

Class Distribution

The distribution of benign and malignant cases was examined to identify potential class imbalance.

Feature Distribution

Histograms were used to analyze feature distributions and identify skewness or unusual patterns.

Feature Relationships

Scatter plots were used to examine relationships between tumor characteristics, including radius_mean and texture_mean.

Correlation Analysis

A correlation heatmap was created to investigate relationships between numerical features and the target variable.

Features such as radius, perimeter, and area showed strong relationships with the diagnosis variable.

3. Feature Engineering

Additional features were created from the original variables to provide the models with more informative representations.

Examples include:

total_mean
compact_ratio
log_area

These transformations were designed to capture additional patterns and improve model representation.

4. Machine Learning Models

The following classification algorithms were implemented:

Model	Purpose
Logistic Regression	Binary classification baseline
Support Vector Machine (SVM)	Non-linear classification using RBF kernel
Random Forest	Ensemble tree-based classification
Gradient Boosting	Sequential tree-based classification
Artificial Neural Network (ANN)	Non-linear deep learning classification

5. Feature Scaling

StandardScaler was applied to models that are sensitive to feature scale, including:

* Logistic Regression
* SVM
* ANN

Tree-based models such as Random Forest and Gradient Boosting do not require feature scaling.

Model Evaluation

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* ROC-AUC

These metrics were used to assess both overall performance and the models’ ability to distinguish between benign and malignant cases.

Results

The project achieved strong classification performance across the tested models.

For the Breast Cancer dataset:

* Logistic Regression: 97.66% accuracy
* Random Forest: 96.49% accuracy
* SVM: approximately 97.4% accuracy
* Random Forest: approximately 97.4% accuracy in the model evaluation experiment

The SVM and Random Forest models achieved excellent AUC scores close to 0.99 in the reported evaluation.

A separate cross-dataset comparison was also conducted using Logistic Regression and Random Forest.

For the binary Iris dataset:

* Logistic Regression: 100% accuracy
* Random Forest: 100% accuracy

This comparison was used to examine how model performance changes across different datasets and problem characteristics.

Artificial Neural Network

The ANN consisted of:

Input Layer  →  32 units, ReLU
Hidden Layer →  16 units, ReLU
Output Layer →  1 unit, Sigmoid

Training configuration:

* Optimizer: Adam
* Loss: Binary Crossentropy
* Epochs: 100
* Batch Size: 16
* Validation Split: 20%
* Early Stopping: Enabled
* Patience: 10
* Restore Best Weights: Enabled

Key Takeaways

This project demonstrates an end-to-end approach to a supervised machine learning classification problem:

Data → Preprocessing → EDA → Feature Engineering → Model Training → Evaluation → Comparison

The results demonstrate that traditional machine learning models can achieve strong performance on structured medical datasets when combined with appropriate preprocessing, feature analysis, and evaluation techniques.

Repository Structure

breast-cancer-classification-ml/
│
├── Breast Cancer Classification Using Machine Learning.ipynb
├── Breast_Cancer_Classification_Machine_Learning.pdf
└── README.md

Skills Demonstrated

This project demonstrates practical experience with:

* Data Cleaning
* Exploratory Data Analysis
* Feature Engineering
* Data Visualization
* Statistical Analysis
* Classification
* Machine Learning
* Deep Learning
* Model Evaluation
* Performance Comparison
* Python
* Scikit-learn
* TensorFlow / Keras

Author

Ola Khalil

Information Systems | Data Analysis | Machine Learning
