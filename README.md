
---

# Lung Cancer Prediction using Random Forest and Comparative Analysis of Other Classification Algorithms

This project leverages machine learning to predict lung cancer risk based on various clinical attributes, focusing on the Random Forest algorithm. The project also includes a comparative analysis of other classification algorithms, such as Logistic Regression, K-Nearest Neighbors (KNN), Multinomial Naive Bayes, and Support Vector Classifier (SVC).

This work is part of a study published in *IEEE Xplore*, detailing our methodology, clinical insights, and evaluation of different models. You can find the full research paper [here](https://ieeexplore.ieee.org/document/10730856).

## Table of Contents
- [Project Overview](#project-overview)
- [Research Paper](#research-paper)
- [Clinical Factors](#clinical-factors)
- [Data Encoding](#data-encoding)
- [Methodology Stages](#methodology-stages)
- [Algorithms Applied](#algorithms-applied)
- [Cross-Validation](#cross-validation)
- [Results and Observations](#results-and-observations)
- [Contributing](#contributing)

## Project Overview
This project aims to build a predictive model using several machine learning algorithms to analyze clinical factors and predict lung cancer risk. The structured methodology involves five main stages and evaluates fifteen significant clinical factors, allowing for a robust approach to assessing and comparing model effectiveness.

## Research Paper

This project is based on our research paper published in *IEEE Xplore*. The paper provides an in-depth study of lung cancer risk prediction using machine learning models. You can access the full research here:

- **Title**: Lung Cancer Prediction using Random Forest and Comparative Analysis of Other Classification Algorithms
- **Authors**: Ujjwal Rajput, [any additional co-authors if applicable]
- **Publication**: IEEE Xplore
- **DOI**: [10.1109/10730856](https://ieeexplore.ieee.org/document/10730856)

## Clinical Factors
The following clinical factors were considered as input features for the predictive models:

- **Age**
- **Gender**
- **Yellow Fingers**
- **Smoking History**
- **Peer Pressure**
- **Anxiety**
- **Fatigue**
- **Allergies**
- **Chronic Disease**
- **Wheezing**
- **Alcohol Consumption**
- **Coughing**
- **Difficulties in Swallowing**
- **Shortness of Breath**
- **Chest Pain**

## Data Encoding

### Original Encoding
The original dataset encoded responses as follows:
- **Yes**: `2`
- **No**: `1`

### Label Encoding
To prepare the data for machine learning algorithms, categorical variables were transformed:
- **Gender**: Female (`0`), Male (`1`)
- **Other Attributes** (e.g., Smoking, Anxiety): Yes (`1`), No (`0`)

## Methodology Stages
The project methodology was organized into the following key stages:

1. **Data Collection**: Gathered relevant clinical data for analysis.
2. **Data Preprocessing**: Encoded categorical variables, removed duplicates, handled missing values, and scaled features where necessary.
3. **Feature Selection**: Selected the most impactful clinical factors to improve model performance based on correlation analysis.
4. **Model Training**: Trained multiple machine learning models and optimized hyperparameters to achieve the best performance.
5. **Model Evaluation**: Evaluated each model using metrics such as accuracy, precision, recall, and AUC score.

## Algorithms Applied
The following machine learning algorithms were applied to predict lung cancer risk:

- **Random Forest (RF)**
- **K-Nearest Neighbors (KNN)**
- **Logistic Regression**
- **Support Vector Classifier (SVC)**
- **Multinomial Naive Bayes**

## Cross-Validation
To ensure robust model evaluation, K-Fold Cross-Validation was initially applied. Given the imbalanced nature of the target variable, **Stratified K-Fold Cross-Validation** was used to maintain consistent class distribution across all folds, helping to minimize potential biases in model training and validation.

## Results and Observations
- **Data Imbalance Handling**: To address imbalanced classes, the ADASYN oversampling technique was used.
- **Feature Engineering**: Created additional features from correlated variables to improve model effectiveness.
- **Model Performance**: Random Forest and SVC performed the best, achieving high accuracy, while Multinomial Naive Bayes had the lowest accuracy.

### Model Accuracy Summary (K-Fold Cross Validation)
| Model                  | Average Accuracy |
|------------------------|------------------|
| Logistic Regression    | 93.2%           |
| K-Nearest Neighbors (KNN) | 92.4%       |
| Multinomial Naive Bayes| 75.2%           |
| Support Vector Classifier (SVC) | 93.9%  |
| Random Forest          | 94.5%           |

For further details on the methodology and a more comprehensive analysis, refer to our published research paper on *IEEE Xplore*: [Lung Cancer Prediction using Random Forest and Comparative Analysis of Other Classification Algorithms](https://ieeexplore.ieee.org/document/10730856).

## Contributing
Contributions are welcome! Feel free to submit a pull request or open an issue for any enhancements or bug fixes.

---