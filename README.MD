# Cardiovascular Heart Disease Prediction Model (Stacking Model)
`Last Updated: 11th February 2023`

### **THIS RESEARCH IS PUBLISHED PLEASE [CLICK HERE](https://doi.org/10.55248/gengpi.2023.4217) FOR READING THE PAPER**

## Dataset Information

### About this dataset:
This dataset contains detailed information on the risk factors for cardiovascular disease. It includes information on age, gender, height, weight, blood pressure values, cholesterol levels, glucose levels, smoking habits and alcohol consumption of over 70 thousand individuals. Additionally it outlines if the person is active or not and if he or she has any cardiovascular diseases. This dataset provides a great resource for researchers to apply modern machine learning techniques to explore the potential relations between risk factors and cardiovascular disease that can ultimately lead to improved understanding of this serious health issue and design better preventive measures

### Aim:
This dataset can be used to explore the risk factors of cardiovascular disease in adults. The aim is to understand how certain demographic factors, health behaviors and biological markers affect the development of heart disease.

### Dataset Description: This dataset contains 70,000 records of patients with the following 13 features:

1. Age: Age of participant (integer)
2. Gender: Gender of participant (male/female).
3. Height: Height measured in centimeters (integer)
4. Weight: Weight measured in kilograms (integer)
5. Ap_hi: Systolic blood pressure reading taken from patient (integer)
6. Ap_lo : Diastolic blood pressure reading taken from patient (integer)
7. Cholesterol : Total cholesterol level read as mg/dl on a scale 0 - 5+ units( integer). Each unit denoting increase/decrease by 20 mg/dL respectively.
8. Gluc : Glucose level read as mmol/l on a scale 0 - 16+ units( integer). Each unit denoting increase Decreaseby 1 mmol/L respectively.
9. Smoke  : Whether person smokes or not(binary; 0= No , 1=Yes).
10. Alco ​­ : Whether person drinks alcohol or not(binary; 0 =No ,1 =Yes ).
11. Active : whether person physically active or not( Binary ;0 =No,1 = Yes ).
12. Cardio ­­ : whether person suffers from cardiovascular diseases or not(Binary ;0 – no , 1 ­‑yes ).

## Basic Outline For A Machine Learning Model:

Points to keep in mind when working with a machine learning model

1. Import the Data
2. Clean the Data
3. Split the Data into Training/Test Sets
4. Create Model
5. Train the Model
6. Make Predictions
7. Evaluate and Improve

## Libraries Needed:

1. Numpy
2. Pandas
3. Matplotlib
4. Scikit-Learn

## Tools Needed:

1. Jupyter (IDE)
2. Github (To pull repository)

## Installation Instructions:

1. Clone the repository.
2. Open terminal and 'cd' to the directory where to saved the repository.
3. Run the command `pip install -r requirements.txt`.
4. Now start working on the repository.

## Methodology:

1. IMPORTING LIBRARIES AND LOADING DATA
2. DATA EXPLORATION
3. DATA PREPROCESSING

    a. Target and Feature values / Train Test Split
4. MODEL BUILDING

    a. KNeighborsClassifier

    b. Linear Support Vector Classification (LinearSVC)

    c. Decision Tree Classifier

    d. Random Forest Classifier

    e. Multi-layer Perceptron classifier

    f. Stacking Classifier

5. Prediction Testing


## In-Depth Working of this model:

### Imports

1. Numpy: For working with arrays.
2. Pandas: Used to analyze the data.
3. OS Module: For working with files/directories.
4. matplotlib: Used for programmatic plot generation.
5. Warnings: Used to control warnings in Python.
6. sklearn: These are simple and efficient tools for predictive data analsis.

### Data Exploration

1. pd.read_csv: Used to load cvs files in pandas dataframe.
2. df.head: It returns first 'n' rows.
3. pd.info: It prints information about the dataframe.
4. df.describe: It generates descriptive statistics.

### Data Preprocessing

1. df.isnull: It detects missing values.
2. df.drop: It drops speficied labels from rows and columns.
3. df.dropna: It drops coloumns and rows where null value is present.

### Model Building

1. KNeighborsClassifier: Classifier implementing the k-nearest neighbors vote.
2. Linear Support Vector Classification (LinearSVC): Similar to SVC with parameter kernel=’linear’, but implemented in terms of liblinear rather than libsvm, so it has more flexibility in the choice of penalties and loss functions and should scale better to large numbers of samples. This class supports both dense and sparse input and the multiclass support is handled according to a one-vs-the-rest scheme.
3. Decision Tree Classifier: Decision Trees (DTs) are a non-parametric supervised learning method used for classification and regression. The goal is to create a model that predicts the value of a target variable by learning simple decision rules inferred from the data features. A tree can be seen as a piecewise constant approximation.
4. Random Forest Classifier: A random forest is a meta estimator that fits a number of decision tree classifiers on various sub-samples of the dataset and uses averaging to improve the predictive accuracy and control over-fitting. The sub-sample size is controlled with the max_samples parameter if bootstrap=True (default), otherwise the whole dataset is used to build each tree.
5. Multi-layer Perceptron classifier: This model optimizes the log-loss function using LBFGS or stochastic gradient descent.
6. Stacking Classifier: Stacked generalization consists in stacking the output of individual estimator and use a classifier to compute the final prediction. Stacking allows to use the strength of each individual estimator by using their output as input of a final estimator.
7.. joblib.dump: It collects all the learning and dumps it in one file.
8. joblib.load: It reconstructs the file for use which is created by 'dump' method.

## Prediction Testing

1. random: It generates random output.

## Acknowledgement
This dataset was provided by the work of [Kuzak Dempsy](https://data.world/kudem).