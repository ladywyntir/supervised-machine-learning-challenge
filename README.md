## Module 19 - supervised-machine-learning-challenge

### Background
Lending services companies allow individual investors to partially fund personal loans as well as buy and sell notes backing the loans on a secondary market.

You will be using this data to create machine learning models to classify the risk level of given loans. Specifically, you will be comparing the Logistic Regression model and Random Forest Classifier.
<hr>

### Consider the models
You will be creating and comparing two models on this data: a logistic regression, and a random forests classifier. Before you create, fit, and score the models, make a prediction as to which model you think will perform better. You do not need to be correct! Write down (in markdown cells in your Jupyter Notebook or in a separate document) your prediction, and provide justification for your educated guess.

**Random Forest Model Definition:** giving each numerical value a category to allow the model to perform with respective features realted to those categories.
**Logistic Regression Model Definition:** with a dependency to calculate based on weights, we can organize the categories given to numerical values by priority, depending on how they're assigned certain numbers.

Random Forest Models do well if the values are close to the range of training data but do poorly if there are extreme outliers. Logistic Regression Models tend to be more accurate as they're based on a mathematical function.

**Prediction: Which Model Will Perform Better?**
Due to the nature of **Logistic Regression** being more objective by using functions rather than closeness of data, I'd predict it would perform better.

<hr>

### Code Theory
1. Pulled in the csv rows into a DataFrame as usual.
2. Looked through the columns to find which would work best as something to catogorize by - loan_status seemed logical and that was confirmed by the assignment rubric.
3. Made my prediction about which would work better - Linear Regression or Random Forest.
4. Split the data into in X Train/Test and y Train/Test.
5. Imported the LogisticRegression function and threw it into a variable.
6. Fit the data into the function and printed it out.
7. Did 1-3 again for the Random Forest notebook.
8. Ran through a for loop so I could import the columns into the DataFrame.
9. Dropped the loan_status column for our X and used it for y (rather than typing out all the columns like in the LinReg notebook).
10. Fit and transformed the data using the Scaler function
11. Ran the model using the transformed data then printed out the scores.
12. Compared my prediction with the results. See below.


<hr>

### Was the prediction correct?

The two models were very close - only differing by a fraction of points. Technically, the Random Forest model did better with the Training score while the Logistic Regression Model did better with the testig score. 


| Logistic Regression Model Results | Random Forest Model Results |
| :---: | :---: |
| Training Data Score: 0.9921240885954051 | Training Score: 0.9975409272252029 |
| Testing Data Score: 0.9918489475856377 | Testing Score: 0.9917457697069748 |
 
![Image](/output/logisticregression_results.png) <br/>
![Image](/output/randomforestclassifier_results.png)