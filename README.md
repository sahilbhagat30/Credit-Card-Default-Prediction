# Capstone-Project-on-Credit-Card-Default-Predictiion

![credit-card-fraudulent-transaction-1024x567](https://github.com/sabitendu/Capstone-Project-on-Credit-Card-Default-Predictiion/assets/117887431/a6773747-e1ee-4be7-b858-7baf635ff584)

## 📋 Introduction
Defaulted credit cards are a significant issue that has negative effects for both banks and customers. If a customer fails to fulfil his commitments, the bank loses money, the customer loses credibility in future payments, collection calls begin, and the case may be taken to court as a last resort. To avoid all of that problems, effective technologies that can anticipate credit card default are required. As a result, default credit card prediction is a significant, difficult, and beneficial issue that must be handled.

Credit card issuers in Taiwan have faced a cash and credit card debt problem in recent years, with delinquency predicted to peak in the third quarter of 2006 (Chou,2006). Card-issuing banks in Taiwan overissued cash and credit cards to unqualified applicants in order to grow market share. Simultaneously, most cardholders, regardless of repayment potential, abused credit cards for consumption and accrued large credit and cash-card debts. The crisis has harmed consumer financial confidence, posing a significant challenge for both banks and cardholders.

## 📋 Abstract
The primary goal is to forecast the likelihood of client default payments in Taiwan. In terms of risk management, the predictive accuracy of the predicted chance of default will be more helpful than the binary categorization result - credible or not credible clients. This would let the issuer decide who to give a credit card to and what credit limit to offer. It would also assist the issuer in developing a better understanding of their current and prospective clients, which would drive their future strategy, including their plans to offer tailored credit products to their customers.
## 📋 Project Files Description
This Project includes 1 colab notebook, 1 technical documentation as well as 1 presentation:

### Executable Files:

*  **Credit Card Default Prediction** - Includes all functions required for clustering operations. Output:
* **Google Colab** - All the outputs are visible in the provided colab notebook. Data Source:
* **Dataset** - Dataset provided by AlmaBetter.

## 📋 Dataset Information:
This dataset contains information on default payments, demographic factors, credit data, history of payment, and bill statements of credit card clients in Taiwan from April 2005 to September 2005. 

There are 25 variables:

* **ID**: ID of each client
* **LIMIT_BAL**: Amount of given credit in NT dollars (includes individual and family/supplementary credit
* **SEX**: Gender (1=male, 2=female)
* **EDUCATION**: (1=graduate school, 2=university, 3=high school, 4=others, 5=unknown, 6=unknown)
* **MARRIAGE**: Marital status (1=married, 2=single, 3=others)
* **AGE**: Age in years
* **PAY_0**: Repayment status in September, 2005 (-1=pay duly, 1=payment delay for one month, 2=payment delay for two months, … 8=payment delay for eight months, 9=payment delay for nine months and above)
* **PAY_2**: Repayment status in August, 2005 (scale same as above)
* **PAY_3**: Repayment status in July, 2005 (scale same as above)
* **PAY_4**: Repayment status in June, 2005 (scale same as above)
* **PAY_5**: Repayment status in May, 2005 (scale same as above)
* **PAY_6**: Repayment status in April, 2005 (scale same as above)
* **BILL_AMT1**: Amount of bill statement in September, 2005 (NT dollar)
* **BILL_AMT2**: Amount of bill statement in August, 2005 (NT dollar)
* **BILL_AMT3**: Amount of bill statement in July, 2005 (NT dollar)
* **BILL_AMT4**: Amount of bill statement in June, 2005 (NT dollar)
* **BILL_AMT5**: Amount of bill statement in May, 2005 (NT dollar)
* **BILL_AMT6**: Amount of bill statement in April, 2005 (NT dollar)
* **PAY_AMT1**: Amount of previous payment in September, 2005 (NT dollar)
* **PAY_AMT2**: Amount of previous payment in August, 2005 (NT dollar)
* **PAY_AMT3**: Amount of previous payment in July, 2005 (NT dollar)
* **PAY_AMT4**: Amount of previous payment in June, 2005 (NT dollar)
* **PAY_AMT5**: Amount of previous payment in May, 2005 (NT dollar)
* **PAY_AMT6**: Amount of previous payment in April, 2005 (NT dollar)
* **default.payment**.next.month: Default payment (1=yes, 0=no)

## 📋 Approaches
On our training dataset, we will begin with basic exploratory data analysis, identifying the data types of features, searching for missing values, scaling some of the features, and encoding categorical variables into usable features. Because we are dealing with a classification problem, we may employ DecisionTree, Logistic Regression,Random Forest, and KNN as supervised learning techniques. As we go through model training, we will fine-tune the hyperparameters of our models and analyse feature importance.

We will re-fit the model on the complete training data set after preprocessing and evaluate its performance on the test data set when we have chosen our final model. To evaluate prediction performance, we will look at overall accuracy as well as misclassifications (from the confusion matrix). We also used Recall and KS-chart to evaluate our final outcomes because they provide a good metric for various criteria.

## **Conclusion**
* We saw that our dataset had an uneven class.
* The majority of credit card holders were female, while male clients had a high default ratio.
* Higher educated people are less likely to default, whereas fewer educated people are more likely to default.
* The likelihood of default increases after the age of 60.
* In this scenario, 'Recall' is a significant parameter to compare all of the algorithms. Because the corporation cannot afford to anticipate a false negative, that is, to predict a defaulter as a non-defaulter. Since the corporation is the one who would deliver money to consumers, if for any reason, sending money to defaulter increases the risk of obtaining the investment returned. As a result, recognising false negatives is critical in this case.
* The Random Forest Classifier model has a high recall (83.89%).
* I will not use KNN as my basic model because it has a similar recall to Random Forest Classisieer, but its bestparams n_neighbors is 1 and can be noisy, leading to outlier effects in the model.

## 📚 References
* Kaggle
* Analytics Vidya
* Towardsdatascience

 ## 📜 Feedback 
 If you have any feedback, please reach out to us at sabitendumahapatra@gmail.com



