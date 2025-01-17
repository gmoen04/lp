# Fake News Detection

I use two datasets, a fake news dataset and true news dataset. I added true and fake labels to them and began the rest of the cleaning process which included the following:

* Converting the text to lowercase, removing punctuation, numbers, and extra spaces
* Removing stop words and additional ‘identifiers’ with regex
* Stemming the words

Feature engineering was done to add additional information to the dataset which might help with classification. In this case, text length and punctuation as a percentage of text were calculated and assessed as features. The former added some useful information while the latter added none and wasn't used in the end. 

After this, data cleaning continued.
* Data transformation for text length
* Splitting the data into training and test sets
* Vectorizing the tokens (TF-IDF)
* Estimating best hyperparameters
* Running and evaluating the random forest and gradient boosting models based on
	* Time taken 
	* Precision
	* Recall
	* Accuracy
	
After all of this was done, the results for both models were visualised in the form of a classification report, a confusion matrix and an ROC curve. 

**Files**
* data_analysis.ipynb
	* The analysis process once the data had been properly cleaned	
* data_cleaning.ipynb
	* The process of getting the data ready for analysis	 	
* dataset_reduced.csv
	* The reduced version of the dataset (used for analysis) of a size suitable for uploading	
