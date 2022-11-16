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
Statistic Analysis has been done such as shapiro wilk normality test and levean test for covariances
Learning Curve has been created to check whether models is overfit or not.
Model analysis is also done for visual analysis of model performance. 


 ### Model comparision
 
As we can see from model evaluation matrices, the accuracy of optimized LDA and QDA model is the same. AUC curve for both model is also the same. Both are good in prediction. As we talk about assumptions, for LDA all independent variables are continuous and look like a bell curve and follow gaussian distribution. All input variables have a same variance. Each of the class has identical covariance matrices. Lastly, linear boundary is required between classifier.
On the other hand, assumptions of  QDA are all independent variables are continuous and look like a bell curve and follow gaussian distribution. All input variables do not need to have a same variance. It is used for non-linear boundary. From the assumptions of LDA and QDA, we just violated assumption for both the algorithms, which is all the independent variables are follow gaussian distribution which are not in our case as we can see from conducting Shapiro-Wilk test. Also, data is not numerical, it is categorical. But from Levene test we get all input variables have the same covariance, which is good for LDA.
The main difference is LDA has few hyperparameters that are important to change to optimized model, where as QDA has no hyperparameter which simple model like a Naïve Biased model. So, We can optimise LDA for better model performance but not QDA. Both are suited for smaller dataset like this dataset.
LDA has better learning curve but in the case of QDA, the learning curve indicates that it has high variance and variables are collinear.
In this case, as Levene test states, the same covariance between variables and also, dataset is smaller. so, LDA performs little bit better.  We can optimised model as more data will added.

#### Conclusion

To conclude, we see from comparison LDA and QDA model gives the same accuracy and AUC curve. Both are performed good.
for the puropse we can use LDA and logistic regression for prediction.
However, we need to add more data for better performance, do hyperparameter tuning for LDA, balance classes and try to get independent variables as normal distributed as possible for the better result of discriminant analysis models.
The more the classes are separable and the more the distribution is normal, the classification result for LDA and QDA will be better.









