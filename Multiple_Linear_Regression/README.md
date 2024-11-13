# Multiple Linear Regression for Salary Prediction

This project demonstrates a Multiple Linear Regression model to predict salaries based on years of experience, education level, and city of residence. By preprocessing data with One-Hot Encoding, feature scaling, and employing gradient descent, this model iteratively finds optimal parameters to minimize the cost function, offering predictions for real-world data points.

## Overview

This project includes:

- **Data Preprocessing**: Encoding categorical data (city of residence) with OneHotEncoder and standardizing features for improved model performance.
- **Model Training**: Using gradient descent to train a multiple linear regression model and minimize the cost function.
- **Model Evaluation**: Calculating cost on both training and test sets to assess performance.
- **Prediction**: Using the model to predict salaries for new data points.

## Dependencies

- **pandas**: For data handling and manipulation
- **numpy**: For numerical operations
- **scikit-learn**: For data preprocessing (OneHotEncoder, StandardScaler, train-test split)
- **matplotlib**: For data visualization

## Dataset

The dataset (Salary_Data2.csv) includes columns:

- **YearsExperience**: Number of years of experience of the individual
- **EducationLevel**: Highest level of education, encoded to numerical values (0, 1, 2) for modeling
- **City**: The city where the individual is employed, represented with One-Hot Encoding
- **Salary**: The target variable, representing annual salary in thousands

## Key Functions and Implementation

### Data Preprocessing

- **Encoding**: Uses `OneHotEncoder` to convert the City feature into binary indicators for three distinct cities, ensuring categorical data is correctly processed for the regression model.
- **Standardization**: Applies `StandardScaler` to scale YearsExperience, EducationLevel, and encoded City features, which stabilizes gradient descent and improves convergence speed.

### Model Training: Gradient Descent

The model iteratively updates parameters (weights and bias) using gradient descent:

- **compute_cost**: Calculates the mean squared error (MSE) as the cost function.
- **compute_gradient**: Computes gradients for weights and bias to guide parameter updates.

### Model Evaluation and Prediction

The model is trained on 80% of the dataset (training set) and evaluated on the remaining 20% (test set) for validation.
```
# Example usage for prediction
x_real = np. array([[5.3, 2, 1, 0], [7.2, 0, 0, 1]])
x_real = scaler.transform(x_real)
y_real = (w_final * x_real).sum(axis=1) + b_final
print("Predicted Salaries:", y_real)
```

## Results

Upon training, the model outputs optimized weights w_final and bias b_final, which are then used to predict salaries based on input features. The MSE of the model provides insight into prediction accuracy on the test set.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

```
This README provides a professional structure with each section formatted for clarity, ideal for GitHub repositories. Adjust any details to match the specifics of your project as needed.
```




