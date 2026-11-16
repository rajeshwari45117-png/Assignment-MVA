# Simple Linear Regression: Salary Prediction

## Project Overview

This project demonstrates **Simple Linear Regression** using Python and
scikit-learn. It models the relationship between an employee's **years
of experience** (independent variable) and **salary** (dependent
variable), then predicts salaries for a held-out test set.

## Objective

Build and visualize a linear regression model that predicts salary from
years of experience.

## Dataset

The notebook loads a file named `Salary_Data.csv`:

``` python
dataset = pd.read_csv('Salary_Data.csv')
X = dataset.iloc[:, :-1].values
y = dataset.iloc[:, -1].values
```

The first column is used as the feature (`X`) and the last column as the
target (`y`). Place `Salary_Data.csv` in the same directory as the
notebook before running it.

## Tools and Libraries

-   Python
-   NumPy
-   pandas
-   Matplotlib
-   scikit-learn

## Workflow

1.  Import NumPy, pandas, Matplotlib, and the required scikit-learn
    classes.
2.  Load `Salary_Data.csv`.
3.  Separate the input feature (`X`) and target (`y`).
4.  Split the data into training and test sets using `test_size=1/3` and
    `random_state=0`.
5.  Create and train a `LinearRegression` model on the training data.
6.  Predict target values for the test data.
7.  Plot the training data and fitted regression line.
8.  Plot the test data and the fitted regression line.

## Run the Project

1.  Clone or download this repository.

2.  Install the dependencies:

    ``` bash
    pip install numpy pandas matplotlib scikit-learn jupyter
    ```

3.  Add `Salary_Data.csv` to the project directory.

4.  Launch Jupyter Notebook:

    ``` bash
    jupyter notebook
    ```

5.  Open `35_simple_linear_regression (1).ipynb` (or rename it to
    `simple_linear_regression.ipynb`) and run all cells.

## Expected Visualizations

-   **Training set:** training observations shown as red points and the
    fitted regression line shown in blue.
-   **Test set:** test observations shown as red points and the model's
    regression line shown in blue.

## Model Details

The notebook uses scikit-learn's `LinearRegression` estimator and fits
it with `regressor.fit(X_train, y_train)`. Test predictions are
generated with `regressor.predict(X_test)`.

## Notes and Limitations

-   The notebook does not calculate or report evaluation metrics such as
    MAE, MSE, RMSE, or R².
-   No numerical prediction results are stored in the notebook outputs,
    so this README does not claim a specific accuracy or salary
    prediction.
-   The project requires the external `Salary_Data.csv` file; it was not
    included with the notebook provided.

## Repository Contents

-   `35_simple_linear_regression (1).ipynb` --- Jupyter notebook
    containing the implementation.
-   `README.md` --- project documentation.
-   `Salary_Data.csv` --- required input dataset (add this file
    separately).

## License

Add a license file if you intend to distribute this project publicly.
