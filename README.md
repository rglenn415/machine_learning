# machine_learning
#### Project Abstract:  
The objective of this project is to extract well defined customer problem descriptions from the Cisco Support Community VPN posts and create a logistic regression machine learning model to predict the classification for any CSC VPN post. To accomplish this the text must be cleaned using natural language processing and represented statistically using TF-IDF, Text Frequency - Inverse Document Frequency. While creating the machine learning model also document the mathematics and learning process performed throughout the project.

Domain Knowledge
First I learned about common problems that occurred in VPNs from Cisco Engineers. By talking with experience Cisco engineers, we learned descriptions of each problem and the thought process to approach each different problem type. This classification knowledge helped the team create hand classified training sets of the machine learning algorithms.

Knowledge Engineering
Simultaneously with the Domain Knowledge, I was learning the theory behind machine learning models and how to apply machine learning with associated packages in Python.

Cleaning Data and Representation
After the initial hand classifications were completed in the Domain Knowledge section, the data was fed into a cleaning function. This removes items like punctuation and capitalization to create the most accurate representation using the Text Frequency-Inverse Document Frequency(TF-IDF) package. TF-IDF aims to find the importance of each word in each individual Cisco Support Community post. 

Machine Learning
Each Cisco Support Community post represented with TF-IDF will be fed into the machine learning model with correlated classifications to create the logistic regression model. Certain improvements were made during this process such as implementing upsampling and adjusting logistic regression parameters to improve accuracy or the model's prediction representation.

Results
Overall, the 5-category logistic regression using the UCSC Dataset 3 looks to promise the most consistent set of results with an accuracy of 69.6%. A possible application of this model would be to predict individual cases to help Cisco engineers with their initial evaluation of each post on the Cisco Support Community.

#### Report Files:  
Ryan's Proposal 12:13:17.txt  
    -Contains detailed breakdown of work done over the project
    
#### Main Files:  
  logistic_regression_test&train.ipynb  
    -Runs logistic regression on the UCSC Dataset 3 Final - Sheet1_clean.csv  
    -Splits set of 200 into 180 training and 20 testing sets  
    -Represents data using TF-IDF 
    -Uses 6 fold stratified cross validation and displays results in confusion matrix and accuracy report   
  
   logistic_regression_upsampled.ipynb  
    -Runs logistic regression on the UCSC Dataset 3 Final - Sheet1_clean.csv  
    -Splits set of 200 into 180 training and 20 testing sets  
    -Represents with TF-IDF  
    -Upsamples training set to highest occurance classification  
    -Runs a single fold validation for accuracy  
    
    
#### Supplementary Files:  
  supervised_cleaning.ipynb  
    -Cleans UCSC Dataset 3 Final - Sheet1.csv to  
      --tokenize  
      --punctuation removed  
      --stopwords removed  
      --words lematized  
    -Outputs as UCSC Dataset 3 Final - Sheet1_cleaned.csv  
  
  random_sample.ipynb  
    -creates a random sample of correctly answered VPN posts after 2016  
    
    
#### Data Sets:  
  UCSC Dataset 3 Final - Sheet1.csv  
    -uncleaned data set contaning 200 posts  
    -used only in the cleaning file  
  
  UCSC Dataset 3 Final - Sheet1_clean.csv  
    -cleaned data set contaning 200 posts  
      --tokenized  
      --punctuation removed  
      --stopwords removed  
      --words lematized  
    
    
    
