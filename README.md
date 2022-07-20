# Loan Data From Prosper
## by Roseland Ambuku


## Dataset
There are 113,937 loans in the original dataset each have 81 different characteristics, such as the loan amount, borrower rate (or interest rate), current loan status, borrower income, and many more.

### Data Assessment and Cleaning

1. Choosing a subset of important features 
2. Dropping duplicated rows on the basis of listing number 
3. Converting the datatypes of TotalTrades and TotalInquiries to int , ListingCreationDate to datetime
4. Removing rows that do not have ProsperRating
5. Filling in missing values of occupation and DebtToIncomeRatio
6. Changing the listing category numeric to string.


## Summary of Findings
The metrics in the dataset that are associated with employment status and the debt-to-income ratio are of particular interest to me, as are the attributes that are most accurate in predicting the borrower's annual percentage rate (APR) for the loan.

I anticipate that the entire loan amount will have a detrimental impact on the loan's APR: the lower the APR, the higher the overall loan amount. I also believe that the loan term, Prosper rating, and work status, in addition to the borrower's stated monthly income, will affect the APR

Employment status and occupation will affect out ProsperRating and loan Amount.

A multimodal distribution of APR appears in the visualization. 0.1 for the tiny peak and 0.2 for the huge peak. There is also a minor peak with a 0.3 center. In addition, between 0.35 and 0.36, there is a highly shaped peak. The APR for most loans is 0.43 or less.
The distribution has a unimodal peak around 0.2 and an atypical peak around 0.25, indicating that most people choose a debt-to-income ratio of 1:4, which is advantageous.

With a high around $6,000 and a stated monthly salary less than $30,000, the distribution of income is substantially skewed to the right. A few outliers between 100K and 50K should be eliminated.

The scatter plot also demonstrates that these two variables are negatively connected, supporting our hypothesis that the lower the APR, the greater the loan amount. The correlation coefficient between the borrower APR and loan initial amount is -0.323. Since borrowers with higher monthly incomes could borrow larger sums of money, the relationship between the loan original amount and declared monthly income makes sense.

The better the rating, the lower the borrower APR. The lowest APRs are offered by borrowers with the highest Prosper ratings. It means that the Prosper rating has a strong effect on borrower APR. Borrowers with better rating also have larger monthly income and loan amount. Employed, self-employed and full time borrowers have more monthly income and loan amount than part-time, retired and not employed borrowers.

There is insufficient information on part-time, retired, and unemployed borrowers for the job status variable to demonstrate how it interacts with term and Prosper rating variables. However, it is clear that word and Prosper rating interact in some way. There are proportionally more 60-month loans with B and C grades. Borrowers with HR ratings can only get loans for 36 months.

A higher rating raises the loan amount. A better rating lowers the borrower APR. It's interesting to note that as Prosper ratings rise from HR to A or higher, the correlation between borrower APR and loan amount changes from being negatively to marginally positively. 

This might be the case since borrowers with A or AA ratings have a propensity to take out larger loans; raising the APR might stop them from doing so and maximize the profit. However, because those with poorer credit tend to borrow less money, a reduced APR might persuade them to do so.

It's interesting to note that for borrowers with HR-C grades, the borrower APR decreases as the borrow period lengthens. However, the APR rises as the length of the loan increases for borrowers with B-AA grades.

Given that the pattern of term is consistent across all ratings, it doesn't appear as though there is an interaction effect between term and rating for declared monthly income. However, there is a relationship between period and rating for loan amount. We can see that a higher Prosper rating results in higher loan amounts for all three terms as well as higher increase amplitudes between terms.

## Key Insights for Presentation

As might be expected at the beginning of a new year, January has the most loans recorded, while April has the fewest loans listed.

With each year that goes by, the number of loans mentioned is increasing.

A multimodal distribution of APR appears. 0.1 for the tiny peak and 0.2 for the huge peak. There is also a minor peak with a 0.3 center. In addition, between 0.35 and 0.36, there is a highly shaped peak. The APR for most loans is 0.43 or less.

The distribution has a unimodal peak around 0.2 and an atypical peak around 0.25, indicating that most people choose a debt-to-income ratio of 1:4, which is advantageous.

The APR has a wide range at various loan amount sizes, but the range of the APR gets smaller as the loan amount grows. Overall, as loan amounts increase, the borrower APR decreases.

The borrower APR declines when the rating gets stronger. The lowest APRs are offered by borrowers with the highest Prosper ratings. It implies that the borrower APR is significantly impacted by the Prosper rating.

The occupation affects the borrower's APR, It is interesting to see that sophomores in college have the highest average rating while students at technical schools have the lowest.

It's interesting to note that for borrowers with HR-C grades, the borrower APR decreases as the borrow period lengthens. However, the APR rises as the length of the loan increases for borrowers with B-AA grades.