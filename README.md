# Analyzing-and-Visualizing-the-World-s-Top-Billionaires
This project analyzes the wealth, industries, and characteristics of the world’s billionaires in 2024. The main objective is to explore patterns and predict whether a billionaire is self-made based on features like net worth, industry, source of wealth, gender, education, and other personal attributes.
# World Billionaires List 2024

## Team Members
| Name             | ID    |
|-----------------|-------|
| Gedamu Ayana     | 1238  |
| Hayimanot Kinde  | 0070  |
| Abye Alemayehu   | 0373  |
| Firehwot Abeje   | 0345  |
| Biniyam Kebere   | 0240  |

## Objective
- Understand patterns in global billionaire distribution.
- Identify key factors associated with self-made wealth.
- Build and compare predictive models for self-made status.

## Introduction
The world’s billionaires hold immense influence over the global economy. This project analyzes a 2024 sample dataset of the world’s richest individuals to explore wealth distribution by country, industry, and source of income, and to predict self-made status using machine learning models. The analysis is conducted using Python in Google Colab, focusing on data exploration, visualization, and predictive modeling.

## Data Preparation
A custom dataset of 2024 billionaires was prepared containing the following attributes:
- Name
- Age
- 2024 Net Worth
- Industry
- Source of Wealth
- Title
- Organization
- Self-Made
- Self-Made Score
- Philanthropy Score
- Residence
- Citizenship
- Gender
- Marital Status
- Children
- Education

Data cleaning included:
- Handling missing values and duplicates
- Ensuring correct data types
- Creating new analytical features such as `IsSelfMadeBinary`, `AgeGroup`, and `WealthGroup`

## Exploratory Data Analysis (EDA)
Visualizations were used to gain insights into billionaire demographics and wealth patterns:
- Top countries by billionaire count
- Net worth distribution
- Industries by total wealth
- Age vs net worth correlation
- Wealth sources (Pie Chart)
- Gender distribution (Pie Chart)

Key Findings:
- The United States dominates in both number and total wealth of billionaires.
- The Technology industry leads in accumulated net worth.
- Self-made billionaires account for a significant portion of the dataset.
- Male billionaires significantly outnumber females in this dataset.

## Feature Engineering & Modeling
**Engineered features:**
- `AgeGroup` (Young, Middle-aged, Senior)
- `WealthGroup` (Medium, High, Ultra-High)
- `IsSelfMadeBinary` (Binary indicator)

Models Built:
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- SVM
- K-Nearest Neighbors
- Gradient Boosting Classifier
- XGBoost Classifier

Models were trained and evaluated using metrics such as Accuracy, Precision, Recall, F1-Score, and Cross-Validation scores.

## Results Summary
| Model                   | Accuracy | Precision | Recall | F1-Score |
|-------------------------|----------|-----------|--------|----------|
| Logistic Regression      | 0.92     | 0.91      | 0.89   | 0.90     |
| Decision Tree            | 0.88     | 0.87      | 0.85   | 0.86     |
| Random Forest            | 0.95     | 0.94      | 0.93   | 0.94     |
| SVM                      | 0.90     | 0.89      | 0.88   | 0.88     |
| K-Nearest Neighbors      | 0.89     | 0.87      | 0.86   | 0.86     |
| Gradient Boosting        | 0.93     | 0.92      | 0.91   | 0.91     |
| XGBoost                  | 0.94     | 0.93      | 0.92   | 0.93     |

Interpretation:
- Random Forest and XGBoost achieved the highest accuracy, demonstrating strong predictive power.
- Logistic Regression performed well but is slightly less accurate on complex patterns.

## Insights & Discussion
- Top Country: United States  
- Top Industry: Technology  
- Most Common Wealth Source: Self-Made  
- Average Age: Around 60 years  

Limitations:
- Dataset size is limited to available public data
- Some features like company revenue or valuation are missing

Future Work:
- Use larger datasets from reliable sources (Forbes, Bloomberg)
- Apply advanced algorithms (Neural Networks, XGBoost, SVR)
- Include time-series analysis of billionaire wealth trends

## Tools and Libraries Used
- Python, Google Colab  
- `pandas`, `NumPy` — data analysis  
- `matplotlib`, `seaborn` — visualization  
- `scikit-learn`, `xgboost` — machine learning  

## Repository Structure
