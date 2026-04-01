📊 Project Summary: Predicting Yes Bank Monthly Closing Stock Price
🔹 Objective

The main goal of this project is to predict the monthly closing stock price of Yes Bank using machine learning techniques.
It also focuses on understanding stock trends, relationships between features, and providing insights for decision-making.

🔹 Dataset Details
Total records: 185 rows
Features:
Date (time-based)
Open price
High price
Low price
Close price (target variable)
🔹 Steps Performed
1. 📥 Data Loading & Understanding
Loaded dataset using Pandas
Checked:
Shape, columns, data types
Missing values → none initially
Duplicate values → none found
2. 🧹 Data Preprocessing
Converted Date column into datetime format
Set it as index for time-series analysis
Sorted data chronologically
Handled missing values using:
Mean (numerical)
Mode (categorical)
3. 📉 Outlier Detection & Removal
Used IQR (Interquartile Range) method
Visualized using box plots
Removed extreme values to improve model performance
4. 📊 Exploratory Data Analysis (EDA)

Performed multiple visualizations:

Line plot → trend of closing price over time
Scatter plot → relationship between Open & Close
Histogram → distribution of closing prices
Heatmap → correlation between features

👉 Key insight:

Strong relationship between Open, High, Low, and Close prices
5. ⚙️ Feature Engineering
Created new features:
Open-Close Difference
High-Low Ratio
Converted categorical data using One-Hot Encoding
Scaled features using StandardScaler
6. 🔗 Multicollinearity Handling
Used VIF (Variance Inflation Factor)
Removed highly correlated features (VIF > 10)
7. 🤖 Model Building
Model used: Random Forest Regressor
Input features: Open, High, Low
Target: Close price
8. 📈 Model Performance
MAE: 8.73
MSE: 190.73
RMSE: 13.81
R² Score: 0.9789

👉 This indicates very high accuracy (model explains ~97.8% variance).

🔹 Key Insights
Stock prices show strong correlation among features
Historical price patterns help in prediction
Random Forest performed very well for regression
Feature importance shows High & Low prices are major contributors
🔹 Conclusion
The project successfully builds a highly accurate predictive model for Yes Bank stock prices
Proper EDA, preprocessing, and feature engineering significantly improved results
The model can be useful for:
Investors
Financial analysts
Stock market forecasting systems
🔹 Future Scope
Use advanced models like:
LSTM (for time-series forecasting)
Add external factors:
Market news
Economic indicators
Deploy as a real-time prediction system
