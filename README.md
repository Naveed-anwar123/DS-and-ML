# DS-and-ML

### Data Reading and Exploration: 

Project is related to data of CARAVAN, an insurance company Data has 86 features and 5822 samples for training and about 4000 samples for testing. Task is to train and find best model for better prediction. Dataset is imbalanced  i.e. 94% zeroes. 
 
### Data Type: 

Data has 41 sociodemographic elements and data cleaning part is almost already done by entertaining all the aspects like categorical and dummies are created for categorical data. Data dictionary has all the information about data.In Target 0 shows that insurance was not availed and 1 shows that customer were given insurance service by caravan.  Solution steps for training and getting best model:  It is classification problem. 

After exploring and visualizing the data features we applied KNN, Random Forest, Naïve based , Logistic regression and decision tree without feature engineering and feature selection. All the models had accuracy of about 94 % on both training and testing data that is not of extreme importance for us as we have imbalanced and data and had mean square error is 0.06 means our model is doing nothing. And instead of seeing accuracy Confusion matrix is of extreme importance for visualizing the results and estimate the model performance. 

Then we applied correlation, Cross validation, all the methods of feature selection,feature importance and applied all the models after each method but none of the classification model has better performance all of the have about ,0.05 to 0.06 mean square error and their confusion matrix shows the bad prediction of ML models. 

### Final Step: 

After training models on all of the above methods and having bad prediction performance of all we explored the concept of sampling and its types for training of models on imbalanced data. Under sampling and over sampling were applied.  
Random under sampler dropped the samples with majority target and equalize proportion of minority(Dataset is shortend) and models started underfitting. <b>TomekLinks</b> drops majority that are near to minority data points 

But still model performance is about same because of less reduction of majority data points. 
Then <b>cluster centroid under sampling</b> was applied: ClusterCentroids is an object that under-samples the majority by replacing cluster of samples by the cluster centroid of a KMeans algorithm.

## Best Solution and model: 

Synthetic Minority Over-sampling Technique 

## Model Performance: 
Random Forest ,logistic regression and decision tree has an CV accuracy of 0.89 and test accuracy without CV is 1. while Naïve bayes model CV accuracy is 1 along with other without CV.  
