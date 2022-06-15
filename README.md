# DDOS_Attack_Detection
Classifying the datalogs/datasets whether malicious or normal using different ML algorithms.

The main objective of this project is to classify a datalog session into Normal or Anomaly. DDOS stands for Distributed Denial of Service attack. I have used various Classification type ML algorithms namely :

    0. Logistic Regression 
    
    1. Random Forest
    
    2. Support Vector Machine - Linear
    
    3. Support Vector Machine - Poly
    
    4. Support Vector Machine - rbf
    
    5. Support Vector Machine - Sigmoid
    
    6. Decision Tree
    
    7. Naive Bayes
    
    8. K-nearest Neighbours
    
As I need to classify the session into 2 categories, This is a Binary Classification Problem.   
## About the Dataset:  
  The dataset consist of 25193 rows with 42 columns. The first 41 columns are about the information on session like No. of Source packets, Protocol type, Flag, No. of logins attempted, etc. The Final Column is the target/Dependent column consisting of whether the session is normal or anomaly.
  
## Walkthrough the files in repository
  ***ddosdet.py*** - The aim in creating this python file is to provide a Menu Driven User Interface for classifying the dataset.  
  ***DDOS_attack_Detection.ipynb*** - As the User Interface is ready, The testing and evaluation as well as hyper parameter tuning of the Machine Learning models are done in this Python Notebook file. Used gridsearchcv and as combination of most commonly used parameters for testing each model. The results obtained through this method are imported as csv files.  
  ***macro-enabled spreadsheets*** - The Results obtained are later used in analysing the models and plotting a line and bar graphs using Excel's inbuilt charts.
  
 ## Results  
 Out of all the Machine learning models:  
Random Forest Classifier has the Best Mean Test Score with a Score of 99.722 with parameters : {'criterion': 'entropy', 'max_features': 'sqrt', 'n_estimators': 30}  
Decision Tree Classifier has taken the least amount of mean time with a Time Period of 0.00412 secs.
      
