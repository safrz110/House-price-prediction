Project Overview
This project focuses on predicting house prices using Machine Learning techniques. The model analyzes various features such as area, number of rooms, location, amenities, and other factors to estimate property prices accurately.

Objective
Build a regression model to predict house prices
Perform data preprocessing and feature engineering
Evaluate model performance using standard metrics

Dataset Information
Total records: 600
Features include:
Area, lot size
Bedrooms, bathrooms, floors
Location, furnishing status, property type
Distance to city, crime rate
Ratings (builder & society)
Amenities (balcony, power backup, etc.)
 
Technologies Used
Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn

 Data Preprocessing
Handled missing values (power_backup filled with mode)
Removed outliers using IQR method
Feature engineering:
total_rooms
area_per_room
bathroom_ratio
luxury_score
location_score
Applied log transformation on target variable (price)
 
Model Pipeline
Numerical features → StandardScaler
Categorical features → OneHotEncoder
Combined using ColumnTransformer
Model used: Linear Regression

 Model Performance
Metric	Value
R² Score	0.8688
MAE	2,915,441
RMSE	4,230,053

 Visualization
Price distribution plot
Correlation heatmap
Actual vs Predicted scatter plot
Key Insights

Top features impacting house prices:
Area (area_sqft)
Location (Urban, Suburban)
Property type (Villa)
Furnishing status
Location score

How to Run
Clone the repository
Install dependencies:
pip install pandas numpy matplotlib seaborn scikit-learn
Run the Jupyter Notebook:
jupyter notebook

 Project Structure
house-price-prediction/
│── House_price_prediction.ipynb
│── house_price.csv
│── README.md

Future Improvements
Try advanced models (Random Forest, XGBoost)
Hyperparameter tuning
Deploy using Streamlit
Add cross-validation

 Author
Sarfaraz Ali

Acknowledgment
This project is built for learning and practicing Machine Learning concepts and real-world data handling.
