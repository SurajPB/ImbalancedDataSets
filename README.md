# ImbalancedDataSets

1. Most of the ML algorithms takes data is equally distributed
2. We are particualry interested in Minority class
3. Imbalance Degree : Ratio of minority class to Majority class
4. If sample size is small finding patterns inherent to the small class is very hard -- imbalanced dataset may not be a problem if the dataset is big enough
5. Class separability : If the classes are overlap each other then its hard to find the rules or boundaries that separate one class to another. Linearly separable domains are not sensitive to any amount of imbalanced dataset, means if the two classes are very clearly linearly separated, then it doesnt really matter if we have imbalaned dataset
6. In many classification problems, a single class is composed of several sub clusters - called as within class -imbalanced where sub-clusters not containing same nunber of examples

# Approaches To Deal with Imbalanced Datasets:
Different approaches works better in different scenarios with different datasets. We can group these appraches into
1. Data level approach --  Modifies Datasets (Changing the distibution of the data to have more observations from the minority class or less observations from the majoruty class, so that we reach similiar ratio each one of the classes).
    Under Sampling -- Random under sampling (decrease the number of observations from the majority at random)
    Over Sampling -- Random over sampling (increases the number of obserations from the minority at random)
    Or create new data that look like minority class like SMOTE
    Try to remove noise or remove those observations which are easy to classify, so that we let the algorithm to focus of harder instances
3. Cost Sensitive Approches -- Modifies the costs we are trying to optimize
   Apply higher costs to the misclassification of the minority class
   different costs to different errors -- we apply higher costs to the misclassification of an instance from the minority respect to an instance of majority. We are changing minimization formula that the model is trying to fit. 
5. Ensemble algothm Approaches -- Leverages the power of building several ML algorithms to predict the minority class in an imbalaced dataset
    Boosting and Bagging
    With Data level approaches to moditfy the original datasets
    Combining classifiers generally improve the generalization ability
   
 
 # Metrics Used to evaluate model performance for Imbalanced datasets
 
 1. Independence of Probability threshold:
      -- ROC - AUC
      --  Precision  Recall curves
 2. Dependent of Probability threshold :
      -- Accuracy (Is not a good metric while evaluating imbalanced datasset : (No. of Correct Prediction / Total no. of predictions)   : as minority class only have less numbers compared to majority class -- model always predicts majority class)
      # Accuracy.ipynb
      
      Loading the data with pandas
      data=pd.read_csv('sample.csv')
      change the ouput label by map function and labelled as target, changing as -1 to 0 and 1 to 1 by the following function
      data['target']=data['target'].map({-1:0,1:1})
      
      
      --  other confusion matrix
             -- Precision 
             -- Recall
             -- F1-score
             -- FPR, FNR
         
 
 
 
    
  





