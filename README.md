# Heart-Disease-Prediction-Using-KNN-Model

This project uses the **k-Nearest Neighbors (k-NN)** algorithm to predict heart disease based on various health metrics. The model was optimized using **Grid Search** for hyperparameter tuning, resulting in improved accuracy on both the training and test datasets.

## Table of Contents

- [Introduction](#introduction)
- [Data](#data)
- [Model Performance](#model-performance)
- [Visualizations](#visualizations)
- [Installation](#installation)

## Introduction

Heart disease is one of the leading causes of death globally. This project aims to develop a machine learning model to predict whether a patient is at risk of heart disease based on key features such as age, cholesterol levels, blood pressure, and more.

By applying the k-NN algorithm and optimizing it through a **Grid Search**, we were able to significantly improve the model's accuracy, making it a useful tool for preliminary health assessments.

## Data

The dataset used in this project is sourced from a CSV file and contains various health indicators such as:

- Age
- Gender
- Chest Pain Type
- Resting Blood Pressure
- Cholesterol
- Maximum Heart Rate
- And more...

The dataset is structured into a pandas DataFrame for analysis and model training.

## Model Performance

After performing a **Grid Search** to optimize the model’s hyperparameters, the model achieved the following performance:

- **Training Accuracy (Cross-Validation):** 73.66%
- **Test Set Accuracy:** 75.33%

Best hyperparameters found:
```json
{
  'algorithm': 'brute',
  'leaf_size': 20,
  'metric': 'chebyshev',
  'n_neighbors': 15,
  'p': 1,
  'weights': 'uniform'
}
```

This represents a significant improvement from our previous model, which had an accuracy of 69.33%. The Grid Search helped fine-tune the model, leading to more reliable predictions without overfitting.

## Visualizations

To better understand the impact of different features, the following visualizations were created:

1. **Bar Chart:** Shows the distribution of key categorical variables like chest pain type and gender.
2. **Heatmap:** Displays the correlation matrix between features, helping to identify strong relationships between variables.
3. **Pie Chart:** Visualizes the proportion of individuals with and without heart disease, providing insight into the dataset's class balance.

These visualizations helped guide feature selection and improve model performance.

## Installation

To run this project locally, you'll need to have Python installed along with the following dependencies:

```bash
pip install pandas
pip install numpy
pip install matplotlib
pip install seaborn
pip install scikit-learn
```


