# Gold Price Prediction Project

This project uses a Random Forest Regressor model to predict gold prices based on historical market data, including features like SPX, GLD, USO, SLV, and EUR/USD.

## Project Overview

The goal of this project is to predict gold prices using historical data. The model was built using the Random Forest Regressor algorithm with an emphasis on high accuracy, achieving an R² score of 98% on the test dataset.

## Dataset

The dataset contains the following columns:
- `Date`: From year 2008 to 2018
- `SPX`: S&P 500 index
- `GLD`: Gold price
- `USO`: Crude oil prices
- `SLV`: Silver price
- `EUR/USD`: Euro to US Dollar exchange rate

No missing values were found in the dataset.

## Steps

1. **Exploratory Data Analysis (EDA)**:
   - Performed basic analysis and verified no null values were present in the data.
   - Examined correlations between features using a correlation heatmap.

2. **Data Preprocessing**:
   - Split the dataset into training and testing sets.

3. **Model Building**:
   - Implemented a Random Forest Regressor model with `n_estimators=100`.
   - Trained the model on the training dataset.

4. **Prediction and Evaluation**:
   - Predicted values on the test dataset.
   - Achieved an R² score of 98%, indicating high accuracy.

5. **Results**:
   - Compared the actual vs. predicted values to assess model performance using plots.

## Conclusion

The Random Forest Regressor model performs exceptionally well in predicting gold prices, capturing 98% of the variance in the test data. Further enhancements could include feature engineering and experimenting with other models for improved accuracy.

## Requirements

- Python 3.x
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib (for visualizations)
  
```python
# Import the necessary libraries
from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestRegressor
from sklearn.metrics import r2_score

