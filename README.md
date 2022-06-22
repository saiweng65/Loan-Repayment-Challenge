# Loan-Repayment-Challenge

Loan lending has been an important business activity for both individuals and financial institutions. Profit and loss of financial lenders to an extent depend on loan repayment. Though loan lending is beneficial for both lenders and borrowers, it does carry a great risk of the inability of the loan receiver to repay back the loan. This inability is termed as loan default. Loan default prediction is a crucial process that should be carried out by financial lenders to help them find out if a loan can default or not. Successful loan default prediction can help financial institutions to decrease the number of bad loan issues and eventually increase profit.

Throughout the years, machine learning algorithms have been used to calculate and predict credit risk by evaluating an individual’s historical data. Literally, this can be locally controlled by following these measures.

1. Credit analysis of potential borrowers should be carried out in ordr to judge the credit risk associated with the borrower and to reach a lending decision.
2. Loan repayments should be monitored and whenever a customer defaults, action should be taken. Thus lender should avoid loans to risky customers, monitor loan repayments, and renegotiate loans when customers get into difficulties.
3. Bad loans can be restricted by ensuring that loans are made to only borrowers who are likely to be able to repay, and who is unlikely to become insolvent.

From business context, we want to reduce the number of bad loan which lead to a loss for the lender. Although from the give dataset, each row represents an accepted loan application or a successfully funded loan. But these loans could still possibly be defaulted by the borrower. Solving this problem can help the lender to identify the loan with higher chance of defaulting and necessary action can be taken in advance.

For this assessment, we want to predict which loan has the high probability of being default based on their financial information and payment history.

# Conclusion

In this assessment, we achieved 95% F1 score in predicting loans that have the high probability of being default based on their financial information and payment history using ensemble learning such as bagging technique like Random Forest and boosting technique like XGBoost. Ensemble learning algorithm helps to improve machine learning model performance by combining several models that allow the production of better predictive performance compared to a single model. Moreover, in our problem, false negative is more expensive than false positive. Hence we have to decide the metric to evaluate the model carefully. In our cases, we used f1 score.

Based on the feature importance generated, we can conclude that the number of payment status such as Rejected, Checked, Cancelled, and None, as well as the number off loan, number of paid off loan, first payment status, and maybe clearfraudscore have higher impact on our model. Hence, these are some important features to look at when predicting the loan status. The lender could also use it as a validation critiria in approval process.

# Future Work

1. Collect more data or use upsampling or downsampling techniques to deal with the imbalanced dataset.

2. Try different model like Logistic Regression or SVM. But more transformations have to be done because skewed data will affect the performance in these model as describe previously. We could try deep learning model to further increase classification performance but deep learning model is just like a black box and is uninterpretable. Usually in busness context, we would like our model to be interpretable.

3. Use more information provided in the clarity_underwriting_variables.csv file. This file provides lots of information, maybe some of them are important and useful to us. Since I am not an expert in this area, I decided to use only the clearfraudscore in this file to avoid curse of dimensionality. But we still can use all of them if we want.
