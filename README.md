Boston Housing Valuation & Price Prediction System
📌 Project Overview
This project involves the development of a Machine Learning Regressor to predict the median value of owner-occupied homes in Boston. By analyzing socio-economic and physical attributes (such as crime rates, number of rooms, and property age), the system provides an automated, data-driven valuation tool to assist real estate stakeholders in determining fair market prices.
The solution utilizes a Random Forest Regressor, achieving an 89% accuracy ($R^2$), significantly outperforming baseline linear models.
📂 Project Structure
HousingData.ipynb: The Jupyter Notebook containing the end-to-end data science workflow (EDA, Preprocessing, Modeling, Evaluation).
HousingData.csv: The dataset used for training and testing.
boston_dashboard.html: An interactive HTML5 dashboard to visualize results and simulate price predictions.
Report of Boston House.pdf: A formal report detailing the 5-phase project lifecycle.
📊 Dataset Details
Source: UCI Machine Learning Repository / Kaggle.
Size: 506 Entries, 14 Features.
Target Variable: MEDV (Median value of owner-occupied homes in $1000s).
Key Features:
RM: Average number of rooms per dwelling.
LSTAT: % lower status of the population.
CRIM: Per capita crime rate by town.
PTRATIO: Pupil-teacher ratio by town.
🛠 Methodology
1. Data Preprocessing
Missing Values: Handled using Median Imputation to remain robust against outliers in columns like CRIM, ZN, and LSTAT.
Splitting: Data divided into 80% Training and 20% Testing sets (Random Seed: 42).
2. Modeling Strategy
Algorithm: Random Forest Regressor (Ensemble Method).
Configuration: 100 Estimators (n_estimators=100).
Justification:
Capable of capturing non-linear relationships (e.g., the diminishing returns of additional rooms).
Robust to outliers (mitigating the impact of extreme luxury properties).
Does not require feature scaling (normalization).
📈 Model Performance
The model was evaluated on unseen test data (20% split).
Metric
Score
Interpretation
R² Score
0.89
The model explains 89% of the variance in house prices.
RMSE
$2.87k
On average, predictions are within $2,870 of the actual price.

💻 How to Run the Dashboard
This project includes a standalone HTML dashboard for presenting results.
Navigate to the directory containing boston_dashboard.html.
Double-click the file to open it in your default web browser.
Features:
View interactive charts for Actual vs. Predicted prices.
Use the Price Simulator to adjust sliders (Rooms, Crime, etc.) and see real-time valuation estimates.
📦 Requirements
To run the analysis notebook, you will need the following Python libraries:
pandas
numpy
matplotlib
seaborn
scikit-learn


👤 Author
Tariq Jamil Data Science Student
