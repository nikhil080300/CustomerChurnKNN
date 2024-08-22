# Classification using K-Nearest Neighbors using Scikit-Learn

This project demonstrates the implementation of the K-Nearest Neighbors (KNN) algorithm using the Scikit-Learn library for a classification problem.

## Dataset Overview
We will use a customer dataset (`teleCust1000t.csv`) which includes various features about customers and their respective categories (`custcat`). The objective is to classify customers into their respective categories based on the provided features.

## Steps Involved

### 1. Importing Required Packages
The following packages are essential for the implementation:
- `numpy`: For numerical operations
- `pandas`: For handling the dataset
- `matplotlib`: For visualization
- `scikit-learn`: For implementing the KNN algorithm and other preprocessing tasks

### 2. Loading the Dataset
The dataset is loaded directly from a URL using `wget` and then read into a Pandas DataFrame.

### 3. Data Preparation
- **Feature Selection:** The relevant features (`region`, `tenure`, `age`, etc.) are selected and converted into a Numpy array.
- **Target Variable:** The target variable is `custcat`.
- **Data Normalization:** The features are normalized using `StandardScaler` to ensure zero mean and unit variance.

### 4. Splitting the Data
The dataset is split into training and testing sets using an 80-20 split.

### 5. Training the KNN Model
- The KNN model is trained with different values of `K` (number of neighbors).
- The model's performance is evaluated by calculating the accuracy for each `K`.

### 6. Model Evaluation
- The accuracy of the model for different values of `K` is plotted.
- The `K` value with the highest accuracy is identified.

## Visualization
A plot is generated to show the accuracy of the model as the number of neighbors (`K`) varies. This helps in identifying the optimal `K` value.

## Conclusion
The best accuracy achieved is highlighted along with the corresponding `K` value.

