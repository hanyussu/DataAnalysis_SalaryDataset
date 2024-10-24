# Data Analysis - Salary Dataset 

## Objective
In this data science project, our main goal was to predict person's salary based on his age, country, years of experience, job title, and education level.

## Dataset
For this analysis, we used the dataset: Name:"Salary dataset based on country and race"/ Source: https://www.kaggle.com/datasets/sudheerp2147234/salary-dataset-based-on-country-and-race. The dataset contains 6703 rows of individuals and 9 columns that each of contain unique characteristic, including age, gender, pay, nation, race, degree of education, number of years of experience, and job title.

## Data Exploration and Insights
- During the exploration phase, we observed there are 9 columns of different features with 6703 rows.
- The first column is the unnamed column which is redundant, hence, I dropped the column for the futher analysis.
- ![Screenshot 2023-08-05 at 12 10 17 AM](https://github.com/CSC380-SU23-UofArizona/final-project-hanyussu/assets/97819533/f9c19c3c-ca35-4b13-b633-9b6163cbc87b)

## Data Preprocessing
To ensure data quality and suitability for modeling, we performed the following preprocessing steps:
- Data Cleaning
- Outlier Detection

## Feature Selection/Engineering
We conducted feature selection/engineering to improve model performance. 
Feature Selection: Chi2
The selected features were:
- Salary
- Education Level
- Age
- Years of Experience

## Model Selection
After analyzing different algorithms, we chose Linear Regression and Random Forest Regression as they are well-suited for this task.
- Random Forest Regression: It's a Supervised machine learning technique combining the principles of both decision trees and randomness to create a robust and accurate    regression model.
- Linear Regression: Supervised machine learning technique, used for predicting continuous numerical values by fitting a linear relationship between input features and    the target variable

## Model Training and Evaluation
The dataset was split into training and testing sets. We used KFold-cross validation method to select the best model. 
- The models were assessed based on R-squared and Root mean squared error, producing the following results:
  - Model 1: R-square: 0.6959 / RMSE: 28454.8138
  - Model 2: R-square: 0.8782 / RMSE: 18006.8631

## Results and Conclusion
Based on the evaluation, Random Forest Regression model is more accurate the Linear Regression model. Since it has the lower and smaller R-squared value and root mean squared error respectively. Plus, Linear Regression model has higher KFold - cros validation score.Hence, we used Random Forest Regression as our prediction model for future salary. In conclusion, as long as we are given three parameters, age, years of experience, education level, we are able to predict people's wage. This result could potentially assist people who want to earn a certain level's salary. All they need to do is to set the amount of money that they want to achieve and look in to those three parameters. Should I go back to school and get a degree (education level), should I keep working in the same industry (Years of experience). 

## Future Recommendations
- For future work, we recommend selecting other models to do model training to further enhance the model's performance and achieve even better results.

## Limitations
It is essential to acknowledge the limitations of our approach and the dataset. Some limitations include time sensitive meaning it works precisly near the released date of the dataset, the larger the dataset the accurate it is.

## Acknowledgments
We would like to express our gratitude to Kaggle, Enfa George (Associate Professor, University of Arizona).

## References
- Feature Selection: https://www.youtube.com/watch?v=6N9H9KxdZdk.
- K-means clustering: https://www.youtube.com/watch?v=lX-3nGHDhQg&t=422s.
- Evaluation Matrics: https://www.youtube.com/watch?v=LbX4X71-TFI&t=274s.
- Multiple Regression with statsmodel: https://www.youtube.com/watch?v=I4yGOYBGfqI.
- Cross validation: https://www.youtube.com/watch?v=fSytzGwwBVw&t=244s.


