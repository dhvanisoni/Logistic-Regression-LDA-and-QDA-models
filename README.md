# Machine-learning-project

### BackGround

I choose Happy_Dataset for this project with 6 explanatory variables and 1 dependent variable. Based on independents variables our model predicts the person’s happiness.
This project is based on creating Logistic Regression model on dataset to predict whether the person is happy or not.
Two discriminant analysis models which are Linear discriminant analysis (LDA) and Quadratic discriminant analysis (QDA) were created for better models comparision.
For the EDA purposed Pandas profiling is created which is an automated EDA library in python.
Apart from the model creation, model analysis has been done for model comaprision and model selection.
 
 
### Analysis Steps

Exploratory data Analysis has been done such as data cleaning and outlier detection method. Tukey is used for the outlier detection.
Automated EDA library imported  - pandas Profilling.
Some insights we get from pandas profile report such as fewer duplicate rows, all variables are categorical and It is not a large dataset.
As we see the warning, some independents variables are highly correlated which indicates multicollinearity. This multicollinearity voilates model assumptions. For example, x3 and x6 are highly correlated with x5 and x4 is also highly correlated with x5. Classes are not much imbalanced in dataset, 77 are class 0 and 66 are class 1.
Dataset has no missing values. 






