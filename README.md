# ISP Churn Prediction with Gradient Boosting

## Project Overview
This repository contains the final project for MAS 648, focused on predicting customer churn for an Internet Service Provider (ISP). The project utilizes feature engineering and ensemble machine learning models (XGBoost, CatBoost) to identify at-risk customers.

**Context:** This project is based on the [Kaggle Internet Service Provider Churn Competition](https://www.kaggle.com/competitions/internet-service-provider-churn).

## Authors
**Lance Pollack, Riley Yee, Noah Chance, Waleed El-Jack**
*MAS648, Miami Herbert Business School*

## Model Development & Selection
We tested a variety of models to determine the best approach for predicting churn:
-   **Baseline/Simple Models**: Logistic Regression, Ridge, Lasso.
-   **Interpretable Models**: Decision Tree (used for initial insights and rule segmentation).
-   **Ensemble Models**: Random Forest, XGBoost, CatBoost.

**Winner: XGBoost**
XGBoost was selected as the final model because it successfully captured nonlinear patterns and feature interactions that simpler models missed.
-   **Performance**: Achieved a cross-validated ROC-AUC of **0.6933** (Kaggle Score: 0.6867).
-   **Key Predictors**: `ContractType_Monthly`, `Autopay`, `ServiceType_Fiber Optic`, and `AccountAgeYears`.

## Files Included
-   **[ISP_Churn_Prediction.ipynb](ISP_Churn_Prediction.ipynb)**: The main Jupyter Notebook containing data loading, EDA, feature engineering, and model training/evaluation.
-   **[ISP_Churn_Prediction_Poster.pdf](ISP_Churn_Prediction_Poster.pdf)**: A comprehensive visual summary of the project. **Refer to this poster for detailed charts, the decision tree visual, model evaluation,and business takeaways.**
-   **train_data.csv** & **test_data.csv**: Dataset files required to run the notebook.

## Installation
To run the code, you will need Python installed along with the dependencies listed in `requirements.txt`.

1.  Clone this repository or download the files.
2.  Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1.  Ensure `train_data.csv` and `test_data.csv` are in the same directory as the notebook.
2.  Open `ISP_Churn_Prediction.ipynb` in Jupyter Notebook or JupyterLab.
3.  Run the cells sequentially to reproduce the analysis.

## Contributing
This is a final project submission and is not actively seeking contributions.
