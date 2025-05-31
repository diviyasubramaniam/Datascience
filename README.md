🏠 House Price Prediction Using Machine Learning
This project predicts house prices using supervised machine learning models: Linear Regression, Decision Tree Regressor, and Random Forest Regressor. The dataset contains housing information for King County, USA.

📂 Dataset
Source: kc_house_data.csv

Description: Contains data on home sales, including features like:

Number of bedrooms, bathrooms

Square footage (living space and lot)

Location (zipcode)

Year built, renovated

Price (target variable)

🔧 Project Structure
bash
Copy
Edit
├── kc_house_data.csv         # Dataset
├── house_price_model.ipynb   # Main notebook with models and visualizations
├── submission.csv            # Predictions (optional)
└── README.md                 # This file
📌 Objective
To build and evaluate machine learning models that can accurately predict house prices based on various features.

🧠 Models Used
Linear Regression

Decision Tree Regressor

Random Forest Regressor

Each model is evaluated using:

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

R² Score

📊 Features Selected
Some of the key features used:

bedrooms, bathrooms

sqft_living, sqft_lot

floors, zipcode

condition, grade

yr_built, yr_renovated

Categorical features were encoded if needed. Irrelevant or high-cardinality features were removed.

🧪 Evaluation Results (example)
Model	MSE	RMSE	R² Score
Linear Regression	4.1e+10	64068	0.70
Decision Tree	1.3e+10	36039	0.88
Random Forest	1.1e+10	33176	0.89

✅ Random Forest performed best on training data.

📈 Visualizations
Scatter plot of Actual vs Predicted Prices

Distribution of feature importances (for tree-based models)

House price correlation heatmap

Predicted vs Actual price over time (if date used)

💡 Future Improvements
Hyperparameter tuning with GridSearchCV or RandomizedSearchCV

Cross-validation to avoid overfitting

Feature engineering: log-transform price, interaction terms

Deploy as a web app using Streamlit or Flask

# Install dependencies
pip install pandas numpy scikit-learn matplotlib seaborn

# Run the notebook
jupyter notebook house_price_model.ipynb
