# Diabetes Prediction Project

## Introduction
This project aims to predict whether a patient has diabetes based on various health metrics. The dataset used for this project contains 768 instances with 9 features, including pregnancy count, blood glucose level, blood pressure, skin thickness, insulin levels, BMI, age, and diabetes pedigree function. The goal is to use machine learning techniques to create a predictive model that classifies individuals as either diabetic or non-diabetic.

## Dataset Description
The dataset used in this project is a CSV file containing 768 rows and 9 columns. The columns are as follows:

- `preg`: Number of pregnancies
- `plas`: Plasma glucose concentration
- `pres`: Diastolic blood pressure
- `skin`: Skin thickness measurement
- `test`: Serum insulin level
- `mass`: Body mass index (BMI)
- `pedi`: Diabetes pedigree function
- `age`: Age of the patient
- `class`: Outcome (0 = non-diabetic, 1 = diabetic)

The dataset is used to build a predictive model for classifying individuals based on the provided features.

| preg | plas | pres | skin | test | mass | pedi  | age | class |
|------|------|------|------|------|------|-------|-----|-------|
| 6    | 148  | 72   | 35   | 0    | 33.6 | 0.627 | 50  | 1     |
| 1    | 85   | 66   | 29   | 0    | 26.6 | 0.351 | 31  | 0     |
| 8    | 183  | 64   | 0    | 0    | 23.3 | 0.672 | 32  | 1     |
| 1    | 89   | 66   | 23   | 94   | 28.1 | 0.167 | 21  | 0     |
| 0    | 137  | 40   | 35   | 168  | 43.1 | 2.288 | 33  | 1     |
| 5    | 116  | 74   | 0    | 0    | 25.6 | 0.201 | 30  | 0     |
| 3    | 78   | 50   | 32   | 88   | 31   | 0.248 | 26  | 1     |
| 10   | 115  | 0    | 0    | 0    | 35.3 | 0.134 | 29  | 0     |
| 2    | 197  | 70   | 45   | 543  | 30.5 | 0.158 | 53  | 1     |

## Data Exploration and Preprocessing
The first step was to load and inspect the dataset. The shape of the dataset is (768, 9), meaning there are 768 instances and 9 features. Here is a preview of the first 10 rows of the dataset:


### Data Types:
The dataset contains numeric values, with most columns being of integer or float type.

### Descriptive Statistics:
A statistical summary of the dataset provides an overview of the data distribution:
- The mean, standard deviation, and other statistics for each column are shown.
- The data contains various ranges for features like age, BMI, and blood glucose.

### Class Distribution:
The dataset has a binary classification target, with the class values representing whether a person is diabetic (`1`) or non-diabetic (`0`). The distribution of the classes is:


## Model Development and Evaluation
In this project, machine learning models were developed to predict diabetes. The following steps were followed for model training and evaluation:
1. Data preprocessing (such as handling missing values and normalizing the data).
2. Splitting the data into training and testing sets.
3. Building and training a machine learning model.
4. Evaluating the model using accuracy, precision, recall, and other metrics.

## Results
After training the model, the performance metrics were calculated. The model’s accuracy and precision can help assess how well it classifies diabetic and non-diabetic individuals.

## Conclusion
This project demonstrates the ability to predict diabetes using various health-related features. The predictive model can be further optimized by exploring more advanced techniques, feature engineering, and tuning hyperparameters. Future improvements could include testing different machine learning models and evaluating their performance on this dataset.

## Potential Improvements:
- **Data Imbalance**: The dataset is slightly imbalanced with more non-diabetic individuals than diabetic ones. Techniques like oversampling, undersampling, or using class weights could help address this issue.
- **Feature Engineering**: Additional features such as family history, ethnicity, or other clinical data could improve the model's performance.
- **Advanced Models**: More complex models, like Random Forest, Support Vector Machines, or Neural Networks, could be explored for improved accuracy.
