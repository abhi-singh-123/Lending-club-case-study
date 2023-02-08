# Lending-club-case-study

### Problem Statement
A bank institution is interested in knowing if they clients applying for a loan will deferred or not.

### Dataset
The dataset is based in information gathered in clients that were granted a loan and consecuently they were classified as 'Fully paid' for not defaulted clients, 'Current' for individuals that are in the process of paying and 'Charged-off' for those who has not paid the installments in due time for a long period of time.

### Steps

#### 1. Familiarization with Data
      This is requred to understand the data, gain the business understanding so that what needs to be done can be planned.
      
#### 2. Cleaning the Data
      This is where the most time is spent in a data science or EDA project. Cleaning steps included dropping not required columns/rows, replacing missing values, outlier treatment.

#### 3. Analysis
      As part of analysis, univariate, segmented univariate and bivariate analysis was done. Following are the observations made:--
      
      # Summary and Insights

#### Univariate Analysis
      - A total of ~13.6% customers in total are defaulters
      - 73% customers went for shorter term loan of 36months term while 27% went for 60 months term loan
      - Interest rate is more densed between 10-15%
      - 10+ years experienced people are more in number who needs loan
      - Majority of borrowers don't have their own house
      - Majority of borrowers are not verified
      - Majority of borrowers income is less than 70k
      - Most of the borrowers didn't have public bankruptcies record
      - Most loans were issued in Q4

#### Segmented Univariate Analysis
      - Most of the loans were taken with the purpose of "Debt Consolidation"
      - The chances to default for 60 months term loan is higher compared to 36 months loan.
      - People with lower salary is more likely to default. Trend shows people with salary between 40k-70k has around 15% chance to default while the one in higher income group of 70k-85k has 11% chance
      - 10+ years experience people fully paid the loan on time.
      - People on rent and mortgage are more likely to default when compared to the one with own house
      - 20% of people with atleast 1 public record bankruptcies couldn't pay the loan while 13% with no public record bankruptcies ended up defaulting
      - Trend shows people with unverified income source are more likely to default.
      - Loan grade 'G' loans has 50% chance of defaulting while Loan Grade 'A' loans has just 5%
      - Higher dti means higher risk to default. dti with value 20-30 has more 16% risk to default¶
      - If the enquiry in last 6 months is higher than 2 is more likely to default
      - Loans issued in May, June and october interestingly has higher defaulters

#### Bivariate Analysis

      - Funded amount was higher for people who defaulted in every income group
      - Higher DTI and funded amount greater than 10k led to more defaulters
      - 4-7 inquiries in last 6 months and higher loan/funded amount(> 12k) leading to more defaulters
      - Customers with interest rate of 20% + and loan/funded amount of 10k+ has more chance to default.
      - Loan/Funded amount > 12k and pupose of loan is 'vacation' is more likely to default
      - Grade 'G' and loan >10k is more likely to default
      - Grade 'G' and interest rate >20 is more likely to default
      - DTI with  20-30 and int_rate 12-14% are  more likely to default
      - 4years employment length with 10k+ loan/funded amount is more likely to default
      - May/june/sep/oct with 10k+ funded or loan amount is more likely to default
      
 #### 4. Recommendations and conclusion
 
 #### Major factors/features that can be used to predict chance of defaulting.
- Verification Status
- home_ownership
- Grades
- Annual income
- DTI
- Employment length

#### Model
- This is a classic case of logistic regression. It's a binary classification problem, A model can be developed using a sigmoid function to predict the probability. A probability > 0.5 can be predicted as defaulter while probabilty < 0.5 can be predicted as non-defaulter.

- Alternatively, a neural network can be with RELU activation functional on the hidden layer and and a sigmoid on the outer layer
