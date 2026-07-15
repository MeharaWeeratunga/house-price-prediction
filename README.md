# House Price Prediction

This project explores the Ames Housing dataset and builds machine learning models to predict house sale prices. The goal was to understand the complete machine learning workflow, from exploring the data and handling missing values to training, evaluating, and comparing different models.

## Dataset

The project uses the Ames Housing dataset from Kaggle, containing 1,460 residential properties with 80 features describing various aspects of each house.

## Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Project Workflow

- Explored and analyzed the dataset
- Handled missing values using feature-specific strategies
- Performed feature engineering
- Encoded categorical variables
- Split the data into training and testing sets
- Trained a Linear Regression model
- Trained a Random Forest Regressor
- Evaluated and compared both models
- Analyzed feature importance
- Saved the trained Random Forest model

## Feature Engineering

Three new features were created during preprocessing:

- **HouseAge** – Age of the house at the time of sale
- **TotalBathrooms** – Combined full and half bathrooms into a single feature
- **TotalSF** – Combined basement, first floor, and second floor living area

## Model Performance

| Metric | Linear Regression | Random Forest |
|-------|------------------:|--------------:|
| MAE | $21,184.56 | $17,356.12 |
| MSE | 4,274,677,893.47 | 843,962,511.87 |
| RMSE | $65,381.02 | $29,051.03 |
| R² | 0.4427 | 0.8900 |

## Feature Importance

The Random Forest model identified **TotalSF** and **OverallQual** as the most influential features when predicting house prices. Other important features included `TotalBathrooms`, `HouseAge`, `YearBuilt`, and `GarageArea`.

## Repository Structure

```text
house-price-prediction/
│
├── data/
├── models/
│   └── random_forest_model.pkl
├── notebooks/
│   └── house_price_prediction.ipynb
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

## What I Learned

This project helped me understand:

- Exploratory Data Analysis (EDA)
- Missing value handling
- Feature engineering
- One-hot encoding
- Train/test splitting
- Regression models
- Model evaluation using MAE, MSE, RMSE and R²
- Feature importance analysis

## Future Improvements

- Tune Random Forest hyperparameters
- Perform cross-validation
- Build a small web application for house price prediction
- Submit predictions to the Kaggle competition