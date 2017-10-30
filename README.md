# Data-Science

## Introduction 

This repository contains the solution of the problem provided by Data Sciece Group (DSG) of IIT Roorkee.

## File Info 
 
 The repository has One DataSet folder which contains the test and train data, and four other files.

 DSG_DateSet_result.csv : This file contains the predicted solution of the problem statement.
 
 Data Description.docx : This file contains the description of all the variables in the data.
 
 Problem Statement : This file contains the Problem Statement and other necessary details.
 
 dsg.ipynb : This file contains the code of the solution in python.
 
 # Problem Statement
 
The dataset includes descriptions of hypothetical samples corresponding to 23 species of gilled mushrooms in the Agaricus and Lepiota Family Mushroom drawn from The Audubon Society Field Guide to North American Mushrooms (1981). Each species is identified as definitely edible, definitely poisonous, or of unknown edibility and not recommended. This latter class was combined with the poisonous one. The aim of this problem is to identify the poisonous and edible class. 
 
 # Solution Explained 
 
 * I have imported necessary libraries and loaded test and train dataset.
 * Analysis of dataset has been done like types of variables present in the dataset, description of dataset etc.
 * There are two kinds of data types present in the datset "Categorical" and "Numerical", I have created saperate dataframe for both the data types.
 * At First categorical data type preprocessing and visualization has been done.
      
      1. Checked if there is any null value presente in the test and train datset so that it can be treated accordingly.
      2. Listed all the categorical variables of each columns.
      3. Then I have ploted stacked bar graph for each column, which contains the information about the quantity of edable and poisonous mushroom in each category.
      4. AfterThat Label encoding has been done for categorical variables and i have combined both test and train label encoded dataset for further processing.
      5. OneHotEncoding has been done on the obtained datset, after that it is saperated.
  
  * Then I have done numerical data type preprocessing and visualization.
      
      1. Pairplot and areaplot between radius and weight has been ploted.
      2. Initially data is skewed, i have done log and square-root operation to decrease the skewness of data.
      3. Scaling of data has been done to improve the model.
   
  * Combined both numerical and categorical datasets.
  * 20 percent of data has been taken from train dataset for cross-validation.
  * I have trained 4 classifier (SVM , XGBOOST, KNN , RANDOM FOREST)
  * Accuracy Score on cross-validation set is really good for XGBOOST and Random Forest.
  * I have chosen XGBOOST as final classifier and Predicted the result.

  Final Predictions have been saved in DSG_DateSet_result.csv file.
     
