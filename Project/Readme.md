Final Project report – Credit card fraud transaction prediction

Steps to run the project:
- Step1: The first step was to import the required libraries.
- Step2: Then we load the data from the source into data frames. Our data set has train data and test data separately, so we have read both the datasets into two different data frames.
- Step3: After reading the two separated datasets we merged the datasets.
- Step4: We wanted to get to know the size of the dataset and their datatypes.
- Step5: Later we checked for null values in the data frame.
- Step6: We found few duplicate entries in our data and dropped them which were not useful.
- Step7: Founded the correlation between the columns and dropped columns if necessary.
- Step8: Next we stored the data into MongoDB using MongoDB compass.
- Step9: After storing data we made a connection to Pyspark through MongoDB.
Step10: Installed Pyspark and using Pyspark we did few of the following steps.
Step11: Created Spark Session.
Step12: We faced issues with the data types in our data so, we used String Indexer for handling categorical values.
Step13: After clearing the issues we created pipelines.
Step14: We split the data into Test data and Train data.
Step15: Then we applied Machine Learning Algorithms using MLlib on the split data.
Step16: Using Logistic Regression method and found accuracy for the data.
Step17: Applying Decision Tree Classifier and showing the accuracy score of the model for the data.
Step18: Implementing Naive Bayes algorithm and finding accuracy score.
Step19: Based on the accuracy scores for different models we can decide which is the best model for the chosen dataset.

Insights From the data:
We have noted some observations while preforming exploratory data analysis on the dataset. We have visualized the data using ‘matplotlib’ and drawn some insights. They are:

1. Based on the amount of fraud transaction happened we came to know the severity of fraud transactions?
2. Total number of fraud transactions occurred?
3. Using Data time column in data set we observed how frequently do fraud transactions occurred.
4. Companies that are more vulnerable to fraud?  - this says merchant categories with high fraud transactions
5. We came to know some facts regarding state wise fraud transactions- Which location has the highest number of fraud transactions.

 Problems Faced: 
* We faced “Py4java” issues while storing the data into mongoDB - We solved it by reinstalling the java and mongoDB with correct versions.
* Machine learning techniques consist of many algorithms, so we were not sure about which algorithms fits for our dataset - We applied few algorithms and based on their accuracy score and time complexity we have decided the best model for the dataset.
* Since our dataset is huge, we faced few java space heap issues - for solving this issue we split the data randomly and used only chunk of it for modeling.

