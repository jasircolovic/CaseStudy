World Happiness Report Analysis

Overview

This project, AID304 - Big Data Analytics: Case Study, analyzes the 2019 World Happiness Report dataset to explore factors influencing happiness scores across countries. The analysis includes data exploration, outlier detection, visualization, and a linear regression model to predict happiness scores based on socio-economic factors.

Dataset





Source: Kaggle (World Happiness Report), accessed via GitHub raw link.



Format: CSV



Description: Contains happiness scores and contributing factors for 156 countries in 2019.



Variables:





Happiness Score



GDP per Capita



Social Support



Healthy Life Expectancy



Freedom to Make Life Choices



Generosity



Perceptions of Corruption



Overall Rank



Country or Region

Analysis Steps





Data Loading and Verification:





Loaded the dataset using pandas and verified its structure (156 observations, 9 variables).



Checked data types and confirmed no missing values.



Data Exploration:





Examined unique values per column to understand data diversity.



Used the IQR method to detect outliers, removing 22 observations, resulting in 134 clean observations.



Visualization:





Created a scatter plot of GDP per Capita vs. Happiness Score to explore their relationship.



Generated a histogram of Happiness Scores to visualize their distribution.



Descriptive Statistics:





Computed measures of central tendency (mean, median) and dispersion (std, min, max) for numeric variables.



Noted moderate variability in Happiness Score (mean: 5.34, std: 0.96) and positive skewness in variables like GDP per Capita.



Regression Model:





Built a linear regression model to predict Happiness Score using six features: GDP per Capita, Social Support, Healthy Life Expectancy, Freedom to Make Life Choices, Generosity, and Perceptions of Corruption.



Split data into 80% training and 20% testing sets.



Results: R-squared of 0.7465 (74.65% variance explained) and RMSE of 0.4231, indicating moderate predictive accuracy.

Key Findings





The model explains 74.65% of the variance in Happiness Scores, suggesting socio-economic factors are significant predictors.



Moderate prediction error (RMSE: 0.4231) indicates the model is effective but could benefit from exploring non-linear relationships or additional features.



Outliers were detected in Social Support, Healthy Life Expectancy, Freedom, Generosity, and Perceptions of Corruption, which were removed to improve model reliability.

Requirements

To run the analysis, ensure the following Python libraries are installed:

pip install pandas numpy matplotlib seaborn scikit-learn

How to Run





Clone this repository or download the code.



Ensure the dataset (2019.csv) is accessible via the specified URL or local path.



Run the script (analysis.py) in a Python environment:

python analysis.py



View the output, including printed results and visualizations.

Future Improvements





Explore non-linear models (e.g., Random Forest, Gradient Boosting) for better predictive performance.



Incorporate additional features or years from the World Happiness Report for a more comprehensive analysis.



Apply feature engineering to capture interactions between variables.

Author





Jasir Colovic



Student project for AID304 - Big Data Analytics
