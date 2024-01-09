# House Price Prediction Using Linear Regression Algorithmn

## Project Overview
Supervised Machine Learning
1. **Dataset:** The source data, encompassing 18 features including square foot of house, number of bedroom, bathroom etc. and its 21,613 observations in King County, USA.

2. **Data Preprocessing:** The dataset underwent preprocessing steps such as handling missing values, encoding categorical variables, and scaling numerical features.
 
3.  **Exploratory Data Analysis:** An exploratory data analysis focuses on the 18 key independent features crucial for prediction and their distribution in the dataset
  
4. **Model Selection and Pipeline:** Linear Regression was chosen as the predictive model, integrated into a pipeline with preprocessing steps and feature selection using Random Selcetion guided by the Statistical Correlation of features yielded same result using SelectKBest. train-test split was performed for balanced class distribution.

5. **Evaluation Metrics:** The model's performance was assessed using R2_score and RMSE, providing insights into its ability to measure the accurately the models level of performance.

6. **Model Improvement:** Feature were further assessed and tuned to produce more better results with the linear Regression Model.

## Usage
To replicate and extend this project, follow these steps:
1. Clone the repository:
`git clone` https://github.com/massivedesigns/House_Price_Prediction_Using_Linear_Regression_Model.git
2. Install the required dependencies:
`pip install -r requirements.txt`

 ## Discussion and Conclusion
 When selecting independent variables based on average or high positive correlation to house prices, the model demonstrated further improved performance, indicating a strong linear relationship with the target variable (house price) with an evaluation score of 0.65, corresponding to 65% accuracy. Further enhancement was achieved by utilising all features in predicting house prices, resulting in a higher evaluation score on test data, reaching 0.70, or 70% accuracy. Subsequent improvements involved an additional data pre-processing step, focusing on the target variable (house price) and the feature with the highest positive correlation (Sqft_living) to the target variable. Applying log transformation to normalize this two features and adding all other features, the model achieved an impressive evaluation score of 0.78, indicating 78% accuracy, with a remarkably low mean square error of 0.0636. This optimized model exhibited close alignment between predicted and actual prices on the test set, making it the most effective in predicting house prices.

 To enhance the model further, recommendations include modifying the data collection process by adding new features. Specifically, incorporating a feature that indicates the presence of luxury in bathrooms could clarify the weight of features like bathrooms, as the current decimal values may not accurately represent their significance in the model. Combining this new feature with the bathroom feature is likely to yield improved results in predicting house prices. Special attention to the square feet of the living area is advised, given its major role in predicting house prices. Additionally, consideration of house grade and the inclusion of a location feature that could replace the latitude and longitude would contribute to the creation of a more high-performing model for the client's future use.
