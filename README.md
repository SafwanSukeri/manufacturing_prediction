# Introduction
The assignment was to build predictive analytics to predict the quality of product at several stages of the process in a manufacturing company. 
# Dataset
The key variables are highlighted in red and green of which the red and green respectively.
The aim of this project is to :
 - Predict variable g4_var_2 using the preceding measurements in the process
 - Define the accuracy of the Predictive Analysis of which the Optimal Value = -0.8574
 - Ascertain the relationship between g4_var_ 2 and g6_var_2, g6_var_3 g6_var_4

![stages of the production process](https://i.ibb.co/n7zXsJp/image1.png)

# Data Pre-Processing
Perform basic data pre-processing methods to ensure data is suitable for any analysis. 

 1. Data Imputation
 2. Exploratory Data Analysis (EDA)
 3. Correlation Analysis
 
![pre-processing result](https://i.ibb.co/vJnmFvc/image3.png)
Figure 2.1 showed a distribution plot of the targeted variable g4_var_2. Due to the presence of missing values in the dataset, the symmetry shape distribution will imply that the missing value is best replaced with the nearest value to the period of missing data (as this is time series data). Next, g1_var_1 and g1_var_3 will be exempted from the analysis due to weak correlation with the targeted variable g4_var_2 which can visualized based on Figure 2.2. In addition, it was discovered that g3_var_3 had only a single value. Hence it will be dropped as well.
Figure 2.3 showcased the 5 out of 9 boxplots of the remaining features. Some of the key findings were, data have been scaled and normalised, outliers were presence in most of the features, g2_var_4 had only 5 values which might implied a categorical variable.

# Methodology
Based on the findings from EDA, the method chose for this analysis will be Regression. The main justifications are explained as follows:
1. Regression models are among the best statistical models for studying relationships between independent and dependent variable for continuous data. This can help the manufacturing company identify key aspect affecting the targeted variable and quality
2. The presence of outliers can be overcome by using Random Forest Regressor Method

# Result
The following is the result of predicting variable g4_var_2 using the preceding variable. 
![result of predictive analysis](https://i.ibb.co/ThVm4BR/image4.png)

 - Random Forest Regressor tend to perform better compared to Linear Regression
 - 𝑅2 Value are 61% and 89% respectively
 - The green region is the Optimum Range based on the given optimum value of -0.8572 ± 1 which is the standard deviation of the variable. The purpose of this Optimum Range is to determine whether the variable g4_var_2 tend to fall within optimum value or otherwise
 - Accuracy to predict such measures for both of the model are 87% and 95% respectively
 - the value of g4_var_2 is affected significantly by the change in the variable g2_var_4.

# Conclusion
The objective of the predictive analysis to predict for any spike (non-optimum) to happen beforehand. This then allows the company to anticipate any anomalies in the future. 
