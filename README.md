# Loan Approval Prediction 
## AIM
This Machine Learning project aims to predict status of loan based on various factors like credit history, applicant's and coapplicant's income, loan term, loan amount, ownership of property etc.

## Dataset
Dataset comprises of training as well as testing dataset. ML models are trained on training dataset and then tested upon the testing dataset.

## ML Models used:
1) Logistic Regression
2) K Neighbors Classifier
3) Random Forest Classifier
4) XG Boost

## Tools and Packages used:
1) Python
2) Pandas
3) Scikit Learn
4) Miceforest
5) Pickle

## Procedure
#### Step 1: Loading and Data Preprocessing of train and test dataset
To load the dataset, the Pandas library was utilised. The target column in the Train dataset—"Loan Status"—has 613 rows and 13 columns. Comparatively, test data is made up of 367 rows and 12 columns. 
There are null values in either dataset. Removing rows with null values could not be beneficial because the dimensionality of the dataset is enormous and practically every row contains some null values. This could shrink our dataset and, in turn, impair model performance. Therefore, null values were imputed using the Miceforest package. Prior to then, integer values were assigned to category variables. 

#### Step 2 : Feature Engineering
Two columns named Applicant's income and Coapplicants income were merged into a single column "Total Income".

#### Step 3: Model Building
Dummy Variable columns were created. To prevent overfitting given the small train dataset, K fold validation was employed in each of the models.
 - Logistic regression with K fold validation
 - Kneighbor Classifier with K fold validation
 - Random Forest with K fold validation
 - XGBoost with K fold validation

#### Step 4: Metrics Selection
Precision score was thought to be a better measure than accuracy because the train dataset is unbalanced, meaning that more loans are authorised than denied.

#### Step 5: Optimization of Models:
Models were optimized with the GridSearchCV to fine tune the best parameters for each of the model

#### Step 6: Selection of the best model and Training
Based on precision score of all 4 models, Random Forest delivered comparatively higher precision score as well as accuracy. Whole of training dataset will trained on Random Forest Model 

#### Step 7: Testing model on Test Dataset 





   







