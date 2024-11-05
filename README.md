# SolarEnergy_Statistics
Machine Learning Project 
## Project Overview
This project analyzes global solar and hydroelectric energy consumption trends across different countries, with a focus on identifying relationships with GDP and population metrics. Using various machine learning models, the project predicts solar energy consumption and energy prices, aiming to provide insights that support the shift toward renewable energy solutions. This project also integrates synthetic data and applies cross-validation techniques to improve model accuracy.
## Objectives
Visualize global energy consumption trends in solar and hydroelectric sectors.
Compare energy consumption patterns with economic indicators like GDP and population.
Forecast future solar consumption using machine learning models.
Predict energy prices using different predictive models.
Enhance prediction accuracy with synthetic data and cross-validation techniques.

## Dataset
The project utilizes datasets containing:

Country-wise energy consumption data, including solar, hydroelectric usage, GDP, and population metrics.
Energy data by Indian state, including energy generation and price metrics.
## Findings and Analysis
Data Preprocessing

Data Cleaning: Addressed missing values and standardized formats.
Feature Scaling: Normalized features for effective model training.
Synthetic Data Generation: Expanded the dataset to improve model robustness.
Visualizations

Trend Analysis: Visualized solar and hydroelectric consumption trends by country.
Comparative Analysis: Explored correlations between GDP/population and solar usage.
Solar Consumption Prediction Models

Random Forest Regressor (RFR): Highest accuracy with R² of 0.65 and MSE of 2,076.75.
ARIMA: Poor performance, with negative R² and high MSE, unsuitable for this data.
Linear Regression: Moderate, explaining 14% of variance; lower accuracy than RFR.
Price Prediction Models

Gradient Boosting: Most accurate for price prediction.
Linear Regression: Strong performance (R² = 0.966, MSE = 5,756.48).
Random Forest Regressor: Lower accuracy (R² = 0.734, MSE = 45,530.25).
Model Optimization

K-Fold Cross-Validation: Reduced overfitting and validated robustness.
Stacking Ensemble: Combined RFR, Gradient Boosting, and Linear Regression to enhance accuracy, especially with synthetic data.
## Conclusion
This study highlights the effectiveness of machine learning in renewable energy forecasting, with ensemble models (Random Forest, Gradient Boosting) outperforming traditional models. The integration of synthetic data and cross-validation further enhances the reliability of predictions. These findings can inform energy policy and support a data-driven transition toward sustainable energy use globally.

## Repository Structure
/SolarEnergy: Contains datasets and jupyter notebooks used for analysis and model training.
/Datasets: Saved datasets for solar consumption and price prediction.


## Getting Started
  ### Clone the Repository:
git clone https://github.com/Shri21cyb/SolarEnergy_Statistics.git
  ### Install Dependencies: Navigate to the project directory and install the required packages:
pip install -r requirements.txt

Run Jupyter Notebooks: Open the notebooks in /notebooks to see data preprocessing, model training, and analysis steps.

## Dependencies
Python 3.7+
Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn, xgboost

## Future Work
Further research can expand on this project by:

Incorporating real-time energy data for improved forecasting.
Extending analysis to include additional renewable sources like wind and biomass.
Developing more detailed geographic-based energy consumption analysis.
