# ImbalancedDataSets

1. Most of the ML algorithms takes data is equally distributed
2. We are particualry interested in Minority class
3. Imbalance Degree : Ratio of minority class to Majority class
4. If sample size is small finding patterns inherent to the small class is very hard -- imbalanced dataset may not be a problem if the dataset is big enough
5. Class separability : If the classes are overlap each other then its hard to find the rules or boundaries that separate one class to another. Linearly separable domains are not sensitive to any amount of imbalanced dataset, means if the two classes are very clearly linearly separated, then it doesnt really matter if we have imbalaned dataset
6. In many classification problems, a single class is composed of several sub clusters - called as within class -imbalanced where sub-clusters not containing same nunber of examples

# ApproachesToDealwithImbalancedDatasets:
Different approaches works better in different scenarios with different datasets. We can group these appraches into
1. Data level approach --  Modifies Datasets (Changing the distibution of the data to have more observations from the minority class or less observations from the majoruty class)
    Under Sampling 
    Over Sampling
3. Cost Sensitive Approches -- Modifies the costs we are trying to optimize
   Apply higher costs to tbe misclassification of the minority class
5. Ensemble algothm Approaches -- Leverages the power of building several ML algorithms to predict the minority class in an imbalaced dataset
    Boosting and Bagging
    With Data level approaches to moditfy the original datasets
    
  





