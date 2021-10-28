# machine_learning-homework

Lending money is a important function in our economy.  Obtaining loans increases consumer and corporate buying power.  Lending institutions use several metrics to determine which potential borrowers are good risks (those who will pay the money back) and which are poor risks (those who will "take the money and run").  

Fortunately, the number of potential good loans outweighs the number of potential bad loans.  This means that the data used to predict loan risk are imbalanced and require preprocessing before a machine learning model can be used to make predictions.

In this repo, there are two Jupyter Lab notebooks.  For the Credit Risk Resampling notebook, I imported a CSV file containing loan data into pandas.  I used scikit-learn to process the data.  First, I transformed the categorical variables into numbers.  Then I split the data into training and testing sets to use in my models.  I normalized the X data using StandardScaler.  

I trained several models and ran metrics for each:

1. Simple logistic regression
2. Oversampling alogrithms - naive random oversampler  and SMOTE
3. Cluster Centroids undersampling algorithm
4. SMOTEENN combination sampling algorithm

I found that each model performed very well with my dataset.

For the Credit Risk Ensemble notebook, I imported another CSV file, this one also containing loan data, into pandas.  I processed the data as in the other notebook.  Then I trained two ensemble classifiers:
 
 1. Balanced Random Forest Classifier
 2. Easy Ensemble Classifier

The Ensemble Classifier performed much better than the Random Forest Classifier.