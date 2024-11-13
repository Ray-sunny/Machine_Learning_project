# Classification Logistic Regression for Diabetes Prediction

## Overview
This project demonstrates a logistic regression model to predict the likelihood of diabetes based on various patient health indicators, including age, weight, blood sugar levels, and gender. The project covers the entire workflow from data preprocessing to model training and evaluation, with gradient descent used to optimize the logistic regression model.

## Dependencies
- **pandas**: For data handling and manipulation
- **numpy**: For numerical operations
- **scikit-learn**: For data preprocessing (StandardScaler, train-test split)
- **matplotlib**: For data visualization

## Dataset
The dataset (`Diabetes_Data.csv`) includes the following columns:
- **Age**: The age of the individual
- **Weight**: The individual's weight in kilograms
- **BloodSugar**: Blood sugar level of the individual
- **Gender**: Encoded as 1 for male and 0 for female
- **Diabetes**: Target variable, where 1 indicates diabetes presence and 0 indicates no diabetes

## Key Functions and Implementation

### Data Preprocessing
- **Encoding**: The `Gender` column is mapped to binary values for model training.
- **Standardization**: `StandardScaler` is applied to standardize the `Age`, `Weight`, and `BloodSugar` features, which stabilizes gradient descent performance.
- **Train-Test Split**: `train_test_split` is used to divide data into training and testing sets (80-20 split).

### Logistic Regression Model
The logistic regression model is implemented from scratch with gradient descent for parameter optimization:
- **Sigmoid Function**: Maps the linear regression output to a probability value, facilitating binary classification.
- **Cost Function**: Binary cross-entropy is calculated to assess the model's performance.
- **Gradient Descent Optimization**: Gradients of weights and biases are calculated and updated iteratively to minimize the cost function.

### Model Training: Gradient Descent
- `compute_cost`: Calculates the cost using binary cross-entropy.
- `compute_gradient`: Computes gradients for the weights and bias for the logistic regression model.
- `gradient_descent`: Iteratively updates weights and bias based on computed gradients and the learning rate.

### Model Evaluation
- **Accuracy**: The trained model is evaluated on the test set to determine its prediction accuracy.
- **Prediction Threshold**: A threshold of 0.5 is used to classify probabilities into binary classes (1 for diabetes, 0 for no diabetes).

### Example Usage for Prediction
The model can be applied to predict diabetes probability for real-world patient data, e.g.:
- **Patient 1**: 72 years, 92 kg, blood sugar 102, female
- **Patient 2**: 62 years, 52 kg, blood sugar 120, male

## Results
The model’s accuracy is evaluated on the test set, and predictions are made for sample patients using the trained model. Results are presented as probabilities of diabetes, indicating the likelihood of each individual having diabetes.

## Usage
1. **Preprocess the Data**: Encode categorical data and scale features.
2. **Train the Model**: Run the gradient descent optimization to minimize the logistic regression cost function.
3. **Evaluate the Model**: Calculate accuracy on the test set and use predictions for new inputs.
4. **Interpret Results**: Based on the probabilities, determine diabetes likelihood for given patients.


