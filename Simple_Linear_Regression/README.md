# Simple Linear Regression Projects

This repository contains two projects that demonstrate linear regression concepts using gradient descent and cost function visualization. Both projects utilize the `Salary_Data.csv` dataset to establish a linear relationship between years of experience and salary, enabling a hands-on understanding of machine learning fundamentals.

## Project Descriptions

### 1. Gradient Descent Project
This project illustrates the process of optimizing parameters in a linear regression model by minimizing the cost function using gradient descent. It involves:
- **Gradient Calculation**: Derives gradients of the cost function with respect to parameters \( a \) and \( b \).
- **Cost Computation**: Calculates the mean squared error as a measure of cost.
- **Parameter Optimization**: Iteratively adjusts parameters to minimize the cost function.
- **Visualization**: Plots the cost against iterations to observe the convergence of the model.

#### Key Functions
- `compute_gradient()`: Computes the gradients for the parameters.
- `compute_cost()`: Computes the cost function value for the current parameters.
- `gradient_descent()`: Performs the iterative gradient descent process, optimizing parameters \( a \) and \( b \).

### 2. Cost Function Visualization Project
This project focuses on visualizing the relationship between the cost function and the parameters \( a \) and \( b \). It highlights:
- **Cost Function Surface**: Creates a 3D surface plot to show how cost changes with different values of \( a \) and \( b \).
- **Optimal Parameters**: Identifies the minimum cost point, highlighting optimal values for \( a \) and \( b \).
- **Interactive Elements**: Uses rotation and view adjustments to better understand the cost function landscape.

#### Key Functions
- `compute_cost()`: Calculates the mean squared error for given parameters, used to generate the cost surface.
- Visualization: Plots the cost function as a 3D surface, displaying cost variations across a range of values for \( a \) and \( b \).

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/simple-linear-regression.git
   cd simple-linear-regression
   ```
2. Install required libraries:
   ```
   pip install pandas numpy matplotlib wget
   ```
## Dependencies

- **pandas**： For data manipulation
- **numpy**：For numerical computations
- **matplotlib**：For data visualization
- **wget**：To download external resources such as font files

## Dataset

The dataset used in both projects is Salary_Data.csv, which consists of two columns: YearsExperience and Salary. This dataset is available in the repository.

## License

This project is licensed under the MIT License.
 ```
This README structure introduces both projects, explains their focus and key functions, and includes setup instructions. It provides clarity for users and potential contributors interested in your linear regression implementations.
 ```



