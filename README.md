## Project Overview
Credit card data, from LendingClub, is used to predict credit risk via analyzing the results of over/undersampling. Recommendations are made regarding the method of sampling to predict credit risk.

## Resources
Data Source: LoanStats_2019Q1.csv.zip

## Results

### Oversampling
-	Naïve Random Oversampling:
		- This model achieves an accuracy score of 64%.
		- The classification report shows:
			- For high risk- 
				- Poor precision 
				- Satisfactory recall 
				- Poor F1 score	
			-For low risk-
				- Great precision
				- Satisfactory recall
				- Satisfactory F1 score
	
-	SMOTE Oversampling:
		- This model achieves an accuracy score of 66%
		- The classification report shows:
			- For high risk- 
				- Poor precision 
				- Satisfactory recall 
				- Poor F1 score	
			- For low risk-
				- Great precision
				- Satisfactory recall
				- Good F1 score

### Undersampling
-	Cluster Centroids:
		- This model achieves an accuracy score of 54%
		- The classification report shows:
			- For high risk- 
				- Poor precision 
				- Satisfactory recall 
				- Poor F1 score	
			- For low risk-
				- Great precision
				- Poor recall
				- Satisfactory F1 score

### Combination Sampling
-	SMOTEENN:
		- This model achieves an accuracy score of 65%
		- The classification report shows:
			- For high risk- 
				- Poor precision 
				- Satisfactory recall 
				- Poor F1 score	
			- For low risk-
				- Great precision
				- Satisfactory recall
				- Satisfactory F1 score

### Ensemble Learners
-	Random Forest: 
		- This model achieves an accuracy score of 68%
		- The classification report shows:
			- For high risk- 
				- Good precision 
				- Poor recall 
				- Satisfactory F1 score	
			- For low risk-
				- Great precision
				- Great recall
				- Great F1 score

-	Easy Ensemble AdaBoost:
		- This model achieves an accuracy score of 93%
		- The classification report shows:
			- For high risk- 
				- Poor precision 
				- Great recall 
				- Poor F1 score	
			- For low risk-
				- Great precision
				- Great recall
				- Great F1 score


## Summary 
	I would not recommend using any of these models to predict both high and low risk credit applicants. Easy Ensemble AdaBoost is the most accurate machine learning model. It can predict low risk applicants with great precision, recall, and a great F1 score. It is however a poor performer when it comes to high credit risk. Random Forest is great at predicting low risk as well and satisfactory at predicting high risk. However, it has a much lower accuracy score than Easy Ensemble AdaBoost. In general, Ensemble Learners were better performers.

