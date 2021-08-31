# Early-NLP-Detection
Early-NLP-Detection for Loan product - Classification issue

## Focus – To Lower NPA (Non Performing Asset)
    
######    Business challenge/requirement
       
- PeerLoanKart is an NBFC (Non-BankingFinancial Company) which facilitates peer to peer loan. (Its not a actual bank, it provides connection between Lender and Borrower)
- It connects people who need money (borrowers) with people who have money (investors). 
- As an investor,you would want to invest in people who showed a profile of having a high probability of paying you back. 
- Ensure NPAs are lower –> meaning PeerLoanKart wants to be very diligent in giving loans to borrower
    NPA - Non-performing asset
- You as a ML expert create a model that will help predict whether a borrower will pay the loan or not. 

###### Business Benifits
- Here we have History data of Loan Borrower repayment/Instalment details. In that few didnt return Loan within the time period and they became Non performing Asset(NPA) to the company. Based on this details, we need to **identify early like who may be going to be such NPA in future**, so that Company can target those cutomer for repayment properly in montly instalment. 
- This will decrease % of becoming NPA and reduceces loss to the company and lender
-  Increase in profits up to 20% as NPA will be reduced due to loan disbursal for only good borrowers

### Loan Eligibility Case Study

#### Here are what the data represent:

* **credit.policy:** 1 if the customer meets the credit underwriting criteria of LendingClub.com, and 0 otherwise.
* **purpose:** The purpose of the loan 
    - (Takes values "credit_card", "debt_consolidation", "educational", "major_purchase", "small_business", and "all_other").
* **int.rate:** The interest rate of the loan, as a proportion (a rate of 11% would be stored as 0.11). 
    - Borrowers judged by LendingClub.com to be more risky are assigned higher interest rates.
* **installment:** The monthly installments owed by the borrower if the loan is funded.
* **log.annual.inc:** The **natural log** of the self-reported annual income of the borrower.
* **dti:** The **debt-to-income** ratio of the borrower (amount of debt divided by annual income, Total Loan/Anual Income--> If its less, its good)).
* **fico:** The FICO credit score of the borrower.
* **days.with.cr.line:** The number of days the borrower has had a credit line.
* **revol.bal:** The borrower's revolving balance (amount unpaid at the end of the credit card billing cycle).
* **revol.util:** The borrower's revolving line utilization rate (the amount of the credit line used relative to total credit available).
* **inq.last.6mths:** The borrower's number of inquiries by creditors in the last 6 months.
* **delinq.2yrs:** The number of times the borrower had been 30+ days past due on a payment in the past 2 years.
* **pub.rec:** The borrower's number of derogatory public records (bankruptcy filings, tax liens, or judgments).

* **not.fully.paid:** This is the **output** field. Please note that **1 means borrower is not going to pay the loan completely**

-  The above problem is a clear classification problem as we need to classify whether the Loan going to be NPA_Status is yes(1) or no(0). So this can be solved by any of the classification techniques like

    > Logistic Regression .

    > Decision Tree Algorithm.

    > Random Forest Technique.
    
    > Gradient Tree Boosting  (Not used here)
    
    > SVM Classifier
    
    > KNN Classifier (Not used here)
    
    > Naive Bayes (But I/P are not independent) (Not used here)
    
    
## Completed Steps:

- Data Cleaning
- Exploratory Data Analysis
- Done Categorial data handling
- Selection of Models: Decision Tree, Random Forest, etc

- Used Initial simple model and hyper parameter tuned model 
- Evaluated the result

- Used Imbalance data handling by SMOTE (Oversampling) + Tomek (Undersampling)
- Evaluated the Models

- Used Scalarization and Imbalance data handling by SMOTE (Oversampling) + Tomek (Undersampling)
-  Evaluated the Models


- **Outcome:By this model reduced the False Negative Errors of such Actual NPA(1) predicted as Non NPA(0)  which is a great advantage for the PeerLoanKart financial company and its customers as well.**


### Conclusion:

- Simple Logistic Regression  is better precision and good confusion metrix after Scaling and Handling Unbalanced data


**Now we  have high recall rate for class =1, we  are able to identify most of NPA candidate early as NPA, So this will help business to target them**

####  Outcome:By this model reduced the False Negative Errors of such Actual NPA(1) predicted as Non NPA(0)  which is a great advantage for the PeerLoanKart financial company and its customers as well.
    

