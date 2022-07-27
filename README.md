# Loan Data From Prosper
## by Roseland Ambuku


## Dataset
Loans Data From Prosper is a dataset with 113,937 records of loans with 81 variables. The variables in the dataset include Loan Status, Listing Category, Borrower State and many more. The records belong to Prosper Bank that issues loans and other banking services to its clients. In this analysis we shall focus on the loan aspect of Prosper Bank's service delivery.

### Data Assessment and Cleaning
The steps taken were:
1. Choosing the subset of features(variables) that are important in the study. 
2. Dropping duplicate values in the dataset
3. Converting the following datatypes:  TotalInquires,InquiriesLast6Months,CurrentCreditLines and OpenCreditLines to int
4. Fill in the missing values of Occupation and DebtToIncomeRatio and EmploymentStatus.
5. Replacing the null values in ProsperScore with the mode
6. Replacing the missing values in the columns below with median values;CurrentDelinquencies,TotalInquiries,InquiriesLast6Months,CurrentCreditLines,OpenCreditLines,AmountDelinquent,DelinquenciesLast7Years,BankcardUtilization,RevolvingCreditBalance.


## Summary of Findings

*Univariate Analysis*
- DebtToIncomeRatio distribution
Most clients of Prosper Bank prefer 1:4 ratio of debt to income evidenced by a peak at 0.25
- Open Credit Lines 
The clients prefer the 5-10 range of Open Credit Lines
- Monthly Income Distribution
The data from the visualization is skewed to the right, with a peak at $5000 which is the common stated monthly income
- Current Credit Lines Distribution
10 is the number of curent credit lines most clients at Prosper Bank have
- Revolving Credit Balance Distribution
0.05 is the revolving credit balance held by the clients of Prosper Bank
- Open Revolving Accounts Distribution
The highest number of Open Revolving Accounts is in the 1 - 9 range and is the preferred range by the bthe clients at Prosper Bank
- The Original Loan Amount
Most clients take out loans of $5k and second preferred loan amount is $10k and the third is $15k. Most loans taken out by clients are in multiples of 5k
- Inquiries in the last 6 months Distribution
0 - 5 is the highest range of Inquiries in the last  months
- Current Delinquencies Distribution
0 - 5 is the highest range of current delinquencies 
- Income Verifiable Distribution
100000 clients of Prosper Bank have verifiable incomes which is the largest portion
- Loan Status Distribution
Current is the most common loan status at Prosper Bank, followed closely by Completed
- Employment Status Distribution
Most of the clients at Prosper Bank are employed, followed closely by those Full time
- Occupation Distribution
'Other' is the most common occupation with Professional a distant 2nd

*Bivariate Analysis*
- Debt to Income Ratio against Loan Status
There is a strong correlation between completed loan statuses and the 1:4 debt to income ratio, which shows most clients within this ratio take out and complete the loan payment.
- Current Delinquencies vs Loan Status
Most of the current delinquencies of accounts have their loans charged off as that is where the strongest correlation lies, 
- Amount Delinquent vs Loan Original Amount
The original loan amounts in the range of $5,000 - $10,000 attracts the highest amount delinquent of $120,000
- Stated monthly income vs Loan Status
Clients of Prosper Bank with $2800 stated monthly income had their loan status cancelled whereas  clients with stated monthly incomes of $6200 have loan status' of Payment in progress

*Multivariate Analysis*
- DebtTo Income Ratio, Income Verifiable and LoanStatus
Few clients of the bank had no verifiable income which is for business, they fall in the categories of Cancelled and Past due by 120 days which explains the case. There is a strong correlation among DebtTo Income Ratio, Income Verifiable and LoanStatus as evidenced by the completed Loan Status which shows most of the clients at the 1:4 debt to income ratio have verifiable incomes and are able to complete loan payments

- Stated Monthly Income, Homeownership of Borrower and Loan Status
Most of Prosper Bank's clients are home owners and few of them are not however this does not impede their ability to pay loans. Most of the clients with the 3 factors, Stated Monthly Income, Homeownership of Borrower and Loan Status, are able to complete their loan paymnets

- Borrower Homeownership, LoanOriginal vs Loan Status
There is a strong correlation among Borrower Homeownership, LoanOriginal and Loan Status at the Current Loan Status which goes to show more clients who own their own homes take out more loans and loans of high amounts. The home serves as a good security for loans and should they default the loan can be recoverd from that security. Home ownership is a good indicater that the client can pay a loan and thus why they take out more loans and high amounts.

## Key Insights for Presentation

Loan Status is the feature of focus in this study as we try to figure out which factors affect this feature. Debt to Income ratio, there is a strong correlation between completed loan statuses and the 1:4 debt to income ratio, which shows most clients within this ratio take out and complete the loan payment. This outcome should encourage the bank to market their loan service to clients who prefer this range for maximum profit on this finanicial product.

With regards to Stated Monthly Income, clients of Prosper Bank with $2800 stated monthly income had their loan status cancelled whereas clients with stated monthly incomes of $6200 have loan status' of Payment in progress. This shows that clients with higher incomes are likely to pay back their loans which calls for the bank to market their loan products to this customer segment.

Prosper Bank should look into debt to income ratio and stated monthly income as metrics to gauge the loan status of thier clients. They should then look into the customer segments that will be found such as high income earners and market their loan products to them and provide incentives to attract and keep that clientele.

The main conclusion is that Prosper Bank should use the factors that affect loan outcomes as a strategy to segment clientele and over a variety of loan products that are tailored to suit the segments. For example from the analysis clients with low stated monthly incomes have most of their loans cancelled which is bad for business. They can turn this around by tailoring a loan product to suit low income earners which will incentivise them to pay their loans and attract other low income earners and bring profit to Prosper Bank.