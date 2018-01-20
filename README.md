# machine_learning

Report Files:
Ryan's Proposal 12:13:17.txt
    -Contains detailed breakdown of work done over the project
    
Main Files:  
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
    
    
Supplementary Files:  
  supervised_cleaning.ipynb  
    -Cleans UCSC Dataset 3 Final - Sheet1.csv to  
      --tokenize  
      --punctuation removed  
      --stopwords removed  
      --words lematized  
    -Outputs as UCSC Dataset 3 Final - Sheet1_cleaned.csv  
  
  random_sample.ipynb  
    -creates a random sample of correctly answered VPN posts after 2016  
    
    
Data Sets:  
  UCSC Dataset 3 Final - Sheet1.csv  
    -uncleaned data set contaning 200 posts  
    -used only in the cleaning file  
  
  UCSC Dataset 3 Final - Sheet1_clean.csv  
    -cleaned data set contaning 200 posts  
      --tokenized  
      --punctuation removed  
      --stopwords removed  
      --words lematized  
    
    
    
