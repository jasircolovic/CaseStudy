# World Happiness Report Analysis 🌍

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

## 📖 Overview
This project, part of **AID304 - Big Data Analytics**, analyzes the 2019 World Happiness Report dataset to uncover insights into factors driving happiness across countries. It includes data exploration, outlier detection, visualizations, and a linear regression model to predict happiness scores based on socio-economic variables.

## 📊 Dataset
- **Source**: [World Happiness Report on Kaggle](https://www.kaggle.com/datasets/unsdsn/world-happiness)
- **Format**: CSV
- **Description**: Happiness scores and contributing factors for 156 countries in 2019.
- **Key Variables**:
  - Happiness Score
  - GDP per Capita
  - Social Support
  - Healthy Life Expectancy
  - Freedom to Make Life Choices
  - Generosity
  - Perceptions of Corruption
  - Overall Rank
  - Country or Region

## 🔍 Analysis Workflow
1. **Data Loading & Verification** 🗂️
   - Loaded dataset using `pandas`.
   - Verified structure: 156 observations, 9 variables.
   - Confirmed no missing values and appropriate data types.

2. **Exploratory Data Analysis** 🔎
   - Checked unique values to assess data diversity.
   - Detected and removed outliers using the IQR method, reducing dataset to 134 observations.

3. **Visualizations** 📈
   - Scatter plot: GDP per Capita vs. Happiness Score.
   - Histogram: Distribution of Happiness Scores.

4. **Descriptive Statistics** 📝
   - Computed mean, median, std, min, and max for numeric variables.
   - Observed moderate variability in Happiness Score (mean: 5.34, std: 0.96) and positive skewness in GDP per Capita and Social Support.

5. **Linear Regression Model** 🤖
   - Predicted Happiness Score using six features: GDP per Capita, Social Support, Healthy Life Expectancy, Freedom, Generosity, and Perceptions of Corruption.
   - Train-test split: 80% training, 20% testing.
   - **Results**:
     - R²: 0.7465 (74.65% variance explained)
     - RMSE: 0.4231 (moderate prediction error)

## ✨ Key Findings
- Socio-economic factors explain ~74.65% of Happiness Score variance.
- Moderate RMSE (0.4231) suggests the model is effective but could improve with non-linear models or additional features.
- Outliers in Social Support, Generosity, and other variables were removed to enhance model reliability.

## 🛠️ Requirements
Install the required Python libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Ensure the dataset (`2019.csv`) is available (via URL or local path).
3. Run the analysis script:
   ```bash
   python analysis.py
   ```
4. Check the console output and generated visualizations.

## 🌟 Future Improvements
- Experiment with non-linear models (e.g., Random Forest, Gradient Boosting).
- Incorporate additional years or features from the World Happiness Report.
- Explore feature interactions for enhanced predictive power.

## 👤 Author
**Jasir Colovic**  
Student project for AID304 - Big Data Analytics

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.