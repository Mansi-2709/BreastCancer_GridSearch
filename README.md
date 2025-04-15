# BreastCancer_GridSearch
## About DataSet

Breast cancer is the most common cancer amongst women in the world. It accounts for 25% of all cancer cases, and affected over 2.1 Million people in 2015 alone. It starts when cells in the breast begin to grow out of control. These cells usually form tumors that can be seen via X-ray or felt as lumps in the breast area.

The key challenges against it’s detection is how to classify tumors into malignant (cancerous) or benign(non cancerous).

This dataset has 569 rows and 32 columns and has following columns 
id                         
diagnosis                  
radius_mean                
texture_mean               
perimeter_mean             
area_mean                  
smoothness_mean            
compactness_mean           
concavity_mean             
concave points_mean        
symmetry_mean              
fractal_dimension_mean     
radius_se                  
texture_se                 
perimeter_se               
area_se                    
smoothness_se              
compactness_se             
concavity_se               
concave points_se          
symmetry_se                
fractal_dimension_se       
radius_worst               
texture_worst              
perimeter_worst            
area_worst                 
smoothness_worst           
compactness_worst          
concavity_worst            
concave points_worst       
symmetry_worst             
fractal_dimension_worst    

The data has a column named 'daignosis' which says whether the tumor is Malignant (which means cell that spreads uncontrollably and is cancerous) or Benign (which means tumors are not usually problematic).

## About the project :

In this project we use the Kaggle dataset. We load the dataset into a pandas dataframe.

We check if there are any null values.We perform EDA on this dataset.

We encode the categorical data and find the coorelation matrix.

Using the coorelation matrix we find all the columns that are highly correlated to our target column i.e. 'diagnosis', so that we can build our model for these features.

We use three ML models i.e. Random Forest,Decision Tree, Logistic Regression to predict about the dataset

We also use GridSearchCv to tune the hyperparameters of the ML models we are using.

We got random_forest as best model and the accuracy score as 0.952569 and the hyperparameters are {'criterion': 'entropy', 'n_estimators': 20}

