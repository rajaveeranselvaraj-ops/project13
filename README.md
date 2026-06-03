Project Overview

This project is a Loan Risk Analysis and Loan Amount Prediction System built using Python.
It performs:

Data loading and preprocessing
Exploratory Data Analysis (EDA)
Risk categorization
Data visualization
Machine Learning prediction using Linear Regression

The system helps financial institutions understand borrower behavior and identify loan default risks.

Features
Load loan dataset using CSV format
Clean and preprocess financial data
Convert categorical values into numerical form
Analyze loan statistics
Detect loan risk categories
Visualize insights using:
Matplotlib
Seaborn
Plotly
Predict loan amount using Machine Learning
Evaluate model performance using:
R² Score
Mean Absolute Error (MAE)
Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Plotly
Scikit-learn
Dataset Columns
Column Name	Description
loan_amnt	Loan amount requested
term	Loan duration
int_rate	Interest rate
annual_inc	Annual income
emp_length	Employment length
home_ownership	Ownership status
purpose	Loan purpose
grade	Loan grade
loan_status	Loan repayment status
Project Workflow
1. Import Libraries

The required Python libraries are imported for:

Data analysis
Visualization
Machine Learning
2. Load Dataset

The loan dataset is loaded using:

pd.read_csv()

The dataset is stored in a Pandas DataFrame.

3. Data Preprocessing
Interest Rate Cleaning

Percentage symbols are removed and converted to float values.

Loan Term Conversion

Loan duration is converted into integer format.

Employment Length Conversion

Employment years are extracted and converted into integers.

Loan Status Encoding
Fully Paid → 0
Charged Off → 1
Label Encoding

Categorical columns are encoded numerically:

home_ownership
purpose
grade
4. Exploratory Data Analysis (EDA)

The project performs:

Dataset inspection
Missing value checking
Statistical analysis
Calculated Metrics
Average loan amount
Average annual income
Average interest rate
5. Data Visualization
Seaborn & Matplotlib Visualizations
Loan default distribution
Annual income distribution
Loan amount distribution
Income vs Loan Amount
Interest Rate vs Loan Status
Correlation Heatmap
Plotly Interactive Visualizations
Loan amount histogram
Risk category scatter plot
Loan status box plot
Loan purpose risk analysis
6. Risk Categorization

Loans are categorized into:

Low Risk
Medium Risk
High Risk

Based on interest rate values:

Interest Rate	Risk Category
< 10	Low Risk
10 – 18	Medium Risk
>= 18	High Risk
7. Machine Learning Model
Algorithm Used
LinearRegression()
Input Features
annual_inc
int_rate
term
Target Variable
loan_amnt
8. Model Evaluation

The model performance is evaluated using:

R² Score

Measures prediction accuracy.

Mean Absolute Error (MAE)

Measures average prediction error.

Sample Output
Model Evaluation
R2 Score: 0.85
Mean Absolute Error: 1200.45
Key Insights
Higher interest rates indicate higher loan default risk.
Annual income influences loan approval amount.
Employment length impacts repayment behavior.
Risk categories help identify potential defaulters.
Loan grading affects lending decisions.
How to Run the Project
Step 1: Install Required Libraries
pip install pandas numpy matplotlib seaborn plotly scikit-learn
Step 2: Run the Python File
python loan_analysis.py
Future Improvements
Use larger real-world datasets
Apply advanced ML models:
Random Forest
XGBoost
Decision Trees
Add accuracy optimization
Deploy as a web application
Create real-time loan prediction dashboard
Conclusion

This project demonstrates how Data Science and Machine Learning can be used in the banking and finance sector to:

Analyze loan applicants
Detect default risks
Predict loan amounts
Support better lending decisions

The combination of visualization and predictive modeling provides meaningful business insights for financial institutions.
