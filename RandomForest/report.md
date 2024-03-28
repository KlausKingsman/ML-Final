# Intro
For this experiment we used Random Forest Classifier to preform binary and multi-classification for this malware dataset.

## Data Processing 
For the data processing part of this expierment, we first outputted the dataset as a dataframe to examine the features that we were dealing with (see data_processing_1.ipynb). We then made two different datasets where one
is the full and unmodified dataset, and the other is a reduced feature dataset to examine if presumed useless or overfitting features from the dataset would merit better results. We can further say that the feature selection library helped us to determine that all the features from the dataset was important. However, upon further examination with the MI scores, we can see that there are three features that have 0.0 MI-score. The features are svcscan.interactive_process_services, handles.nport, pslist.nprocs64bit. However, upon testing this experiment without these features we can see that the results made mininal difference to the experiment with all features. (Note: All features for X is all features without the Class or the Category features). In the Experimentation Section, we will go into detail on how significant the change was and how the experiment was setup. 

## Experimentation/Methodology
In the Methodology, we first grab the dataset and assign X with the features without the Category or Class feature. We took away these features because the Class feature was target one and the Category feature was target two. We also did an experiment with the X variable to be scaled and not scaled. We did a train test split for both X and y variables then ran the dataset through the Random Forest Classifier Algorithm. We then score and proceed to make a confusion matrix of the results, thus following to the Results Section.   

## Results


