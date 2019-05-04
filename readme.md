# Loans: Get Tested Know Your Status
## by D'Jreya Boyd


## Dataset

> There are 113,937 loans and 81 details about each of those loans within the original daataset. The separated data (loans2) consists of the same number of loans, however with only 15(Borrower APR, Borrower Rate, Loan Months Since Origination, Loan Status, Occupation, Employment Status, Employment Status Duration, Monthly Loan Payment , Loan Original Amount, Debt To Income Ratio, IncomeRange, Income Verifiable, Stated Monthly Income) variables. The majority of the variables are quantitative witha few qualitative such as loan status, occupation and income range. Within this data set I will define good standing as Completed or Current for loan status while the remaining options are considered bad standing. 

To begin exploring the data I used panda(.head,.info,.describe, ,shape) methods to visually display the data. From this I noticed how large the dataset was and that there were more columns than I needed. In order to ease the amount of data, I saved only a few of the columns within a new dataframe(loans2). I then replaced all NAN within a column with zeros and saved the change file to a new copy of loans 2 named loans2_clean. I then changed Term, Loan Status, and Employment Status to Category. This was to make it easier to reference within the visualizations lower.


## Summary of Findings

> While creating visualizations I found that most of the distributions I graphed were skewed with the exception of the histogram for Borrower Rates. Even the distribution of loan status was heavily disproportionate. Few of the loans fell within the bad standing statueses. I found the relationship between the loan original amount and the Borrower rate also interesting, it was a right skewed distribution. Within the good standing statuses the range for the borrower rate is actually much wider than the range within in all of the reamining statuses. Meaning the loans with the good status contain both the minimum and the maximum values for the borrower rates.

## Key Insights for Presentation

> For the presentation I focus on the effect of several variables on the loan original amount and loan status. I begin with a univariate exploration of loan status to see a visual of the distribution. From this I notice that more than half of the data is contained within two statuses. Meaning the majority of the loans are well taken care of, Next I do a bivariate exploration of loan status versus term. Within this I see that there are few 12 month terms and most of the good standings are for the 36 and 60 month terms. The longer duration ma make the payments lower allowing an ease in paying back the loans. The final visualisation is for the loan original amount by borrower rate with term as the color encoding. Within this I notice the distribution is heavier on the left side. Closer to the lower loan amounts the data is more stacked and higher borrower rates are more likely. For loans above 25000 it is common to have either a 36 month or 60 month. Higher loan, term period and lower borrower interest rates seems to be the pattern within this plot. I used scatter plot with coor encoding for the final visualization, bar graph and color encoding for the second visualization, and a histogram for the initial 
