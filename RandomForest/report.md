# Intro
For this experiment we used Random Forest Classifier to preform binary and multi-classification for this malware dataset.

## Data Processing 
For the data processing part of this expierment, we first output the dataset as a dataframe to examine the features that we were dealing with (see data_processing_1.ipynb). We then made two different datasets where one is the full and unmodified dataset, and the other is a reduced feature dataset to examine if presumed useless or overfitting features from the dataset would merit better results. We can further say that the feature selection library helped us to determine that all the features from the dataset was important. However, upon further examination with the MI scores, we can see that there are three features that have 0.0 MI-score. The features are svcscan.interactive_process_services, handles.nport, pslist.nprocs64bit (see feature_selection.ipynb). However, upon testing this experiment without these features we can see that the results made mininal difference to the experiment with all features. (Note: All features for X is all features without the Class or the Category features). In the Experimentation Section, we will go into detail on how significant the change was and how the experiment was setup. 

## Experimentation/Methodology
In the Methodology, we first grab the dataset and assign X with the features without the Category or Class feature. We took away these features because the Class feature was target one and the Category feature was target two. We also did an experiment with the X variable to be scaled and not scaled. We did a train test split for both X and y variables then ran the dataset through the Random Forest Classifier Algorithm. We then score and proceed to make a confusion matrix of the results, thus following to the Results Section. Upon experimentation, we seem to see some over fitting with binary classification and this is exaggerated when switching the target to be the Category feature with multiple classifications. We did cross validation to see if the model was indeed generalizing well and we can confirm that the model generalized well with the binary task but not as well with the categorical task. We can further verify this point by running the model with less features from least important feature to most important feature according to the MI scores. The model seems to have consistant accuracy until it only has 9 features left for the binary task. Whereas, the Category task was around the same outcome until it had 15 feature to work with. 

## Results
As a result, the Random Forest classifier was a competative model as it did exectionally well with binary tasks, whereas, the model did decently well with categorical task. 

Binary: 0.999997155697138631
Categorical: 8724614596962285

What we found intresting is that the model seemed to classify benign samples extremely well as according to the confusion matrix there are zero misclassifications of this category, but anything that is not benign was not as accurate. This would basically explain why the model did so well in defining the benign and malware classes in the binary task dispite the help of a categorical feature.  

