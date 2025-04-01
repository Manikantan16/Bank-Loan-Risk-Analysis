# EDA : Bank Loan Default Risk Analysis

### Overview:
- This case study aims to give an idea of applying EDA in a real business scenario.
- In this case study, we will develop a basic understanding of risk analytics in banking and financial services and understand how data is used to minimise the risk 
  of losing money while lending the loan to the customers.
    
### Business Understanding:
-  The loan providing companies find it hard to give loans to the people due to their insufficient or non-existent credit history.
-  Because of that, some consumers use it as their advantage by becoming a defaulter.
-  Suppose you work in a consumer finance company which specialises in lending various types of loans to urban customers, You have to use EDA Techniques to analyse 
   the patterns present in the data.
-  This will ensure that the applicants capable of repaying the loan are not rejected.

When the company receives a loan application, the company has to decide for loan approval based on the applicant’s profile.

### Two types of risks are associated with the bank’s decision:
  1. If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company.

  2. If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company.

### The data given below contains the information about the loan application at the time of applying for the loan. It contains two types of scenarios:

  1. The client with payment difficulties: he/she had late payment more than X days on at least one of the first Y instalments of the loan in our sample.

  2. All other cases: All other cases when the payment is paid on time.

### When a client applies for a loan, there are four types of decisions that could be taken by the client/company:

  1. Approved: The Company has approved loan Application.

  2. Cancelled: The client cancelled the application Sometime during approval. Either the client changed her/his mind about the loan or in some cases due to a higher
     risk of the client he received worse pricing which he did not want.

  3. Refused: The company had rejected the loan (because the client does not meet their requirements etc.).

  4. Unused offer: Loan has been cancelled by the client but on different stages of the process.

### Tools:
  -  Jupyter Notebook.
### Libraries:
  - Numpy,Pandas,Matplotlib,Seaborn.
    
### Conclusion:
After analysing the datasets, there are few attributes of a client with which the bank would be able to identify if they will repay the loan or not.

The analysis is consised as below with the contributing factors and categorization.

  ### Decisive Factor whether an applicant will be Repayer:
  - NAME_EDUCATION_TYPE: Academic degree has less defaults.
  - NAME_INCOME_TYPE: Student and Businessmen have no defaults.
  - REGION_RATING_CLIENT: RATING 1 is safer.
  - ORGANIZATION_TYPE: Clients with Trade Type 4 and 5 and Industry type 8 have defaulted less than 3%
  - DAYS_BIRTH: People above age of 50 have low probability of defaulting
  - DAYS_EMPLOYED: Clients with 40+ year experience having less than 1% default rate
  - AMT_INCOME_TOTAL:Applicant with Income more than 700,000 are less likely to default
  - NAME_CASH_LOAN_PURPOSE: Loans bought for Hobby, Buying garage are being repayed mostly.
  - CNT_CHILDREN: People with zero to two children tend to repay the loans.
    
### Decisive Factor whether an applicant will be Defaulter:
- CODE_GENDER: Men are at relatively higher default rate
- NAME_FAMILY_STATUS : People who have civil marriage or who are single default a lot.
- NAME_EDUCATION_TYPE: People with Lower Secondary & Secondary education
- NAME_INCOME_TYPE: Clients who are either at Maternity leave OR Unemployed default a lot.
- REGION_RATING_CLIENT: People who live in Rating 3 has highest defaults.
- OCCUPATION_TYPE: Avoid Low-skill Laborers, Drivers and Waiters/barmen staff, Security staff, Laborers and Cooking staff as the default rate is huge.
- ORGANIZATION_TYPE: Organizations with highest percent of loans not repaid are Transport: type 3 (16%), Industry: type 13 (13.5%), Industry: type 8 (12.5%) and 
  Restaurant (less than 12%). Self-employed people have relative high defaulting rate, and thus should be avoided to be approved for loan or provide loan with higher 
  interest rate to mitigate the risk of defaulting.
- DAYS_BIRTH: Avoid young people who are in age group of 20-40 as they have higher probability of defaulting
- DAYS_EMPLOYED: People who have less than 5 years of employment have high default rate.
- CNT_CHILDREN & CNT_FAM_MEMBERS: Client who have children equal to or more than 9 default 100% and hence their applications are to be rejected.
- AMT_GOODS_PRICE: When the credit amount goes beyond 3M, there is an increase in defaulters.
