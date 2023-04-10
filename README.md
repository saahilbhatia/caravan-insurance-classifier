# caravan-insurance-classifier
## Description
The key objectives of the project were to predict the most prospective customers for a mobile home insurance policy and explaining why these customers are more likely to buy the insurance policy.

The first task in the project was the prediction task. The objective of this task was to identify 800 customers out of 4000 customers in the test data set with the highest propensity to buy the caravan insurance. 3 Datasets were provided for the task: training dataset, test dataset and the targets dataset. Several classification models - logistic regression, Linear Discriminant Analysis, and Quadratic Disriminant Analysis, were fitted on the training set of the training dataset. The validation set of the training dataset was used to make predictions based on the curves fitted for the training set. The fitted models were compared against each other and the best model used to identify the 800 potential caravan insurance buyers in the test dataset.

The second task in the project was to provide the justification for the prospective customers identified in the prediciton task. The key insights from the chosen classification model backed up with supporting analysis was provided to justify why the company should target the identified customers for their caravan insurance policy.

## Dataset
The dataset used is freely available online at https://kdd.ics.uci.edu/databases/tic/.

It contains about 10K customer records, each of which have 86 attributes. The last attribute indicates if a customer actually bought the caravan insurance. It has been split into training and testing sets. The training set contains 5822 records, and the testing set contains 4000 records.
The training and testing files are stored in three different txt files below:

TICDATA2000.txt : Dataset to train and validate prediction models (5822 customer records). Each record consists of 86 attributes, containing socio-demographic data (attribute 1-43) and product ownership (attributes 44-86).The socio-demographic data is derived from zip codes. All customers living in areas with the same zip code have the same socio-demographic attributes. Attribute 86,\CARAVAN: Number of mobile home policies", is the target variable, indicated by \V86" in the txt file.

TICEVAL2000.txt : Dataset for predictions (4000 customer records). It has the same format as TICDATA2000.txt, only the target is missing.

TICTGTS2000.txt Targets for the evaluation set. 

In the datasets, each line corresponds to a record with tab delimited fields. The name of the attribute contains a letter V followed by an integer that
ranges from 1 to 86. The data dictionary for the dataset is available at https://kdd.ics.uci.edu/databases/tic/dictionary.txt.
## Required packages in R
* ggplot2
* lattice
* caret
* MASS
* boot
* data.table
