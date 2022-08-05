# Loan Data Exploration
## by Carla Aluvai


## Dataset

There are 113,937 loans with 81 features, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. The dataset was provided by Udacity through this [link](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1581581520570000), the feature descriptions are available [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0).


I am interested in finding out the features that can be used to best predict the LoanOriginalAmount feature.

#### Features in the dataset that will help support my investigation into the feature(s) of interest

I suspect that the credit score will have the highest effect on the loan amount given to a borrower.

**Features of Interest Description**
* **IncomeRange**: The income range of the borrower at the time the listing was created.
* **LoanOriginalAmount**: The origination amount of the loan.
* **IncomeVerifiable**: The borrower indicated they have the required documentation to support their income.
* **LoanKey**: Unique key for each loan. This is the same key that is used in the API.
* **CreditScoreRangeLower**: The lower value representing the range of the borrower's credit score as provided by a consumer credit rating agency.
* **StatedMonthlyIncome**: The monthly income the borrower stated at the time the listing was created.
* **ProsperScore**: A custom risk score built using historical Prosper data. The score ranges from 1-10, with 10 being the best, or lowest risk score.  Applicable for loans originated after July 2009.
* **Investors**: The number of investors that funded the loan.
* **IsBorrowerHomeowner**: A Borrower will be classified as a homowner if they have a mortgage on their credit profile or provide documentation confirming they are a homeowner.





## Summary of Findings

Throughout the exploration I found that the income range does influence the loan amount positively. Additionally, it showed that the income verifiable and isborrowerhomeowner feature impacts the loan amount positively depending on the income range. On the other hand, the investord, credit score, the stated monthly income, and the prosper score features had a very weak positive relationship with the loan amount. Ultimately, I found that the income range is the biggest predictor of the loan amount. Every income range has a threshold of how high the loan amount goes even though they all have the same minimum amount. I also noticed that there are other different factors influencing the loan amount in each of the income ranges. But generally, homeowners and those whose income is verifiable tend to have high average loan amounts.


## Key Insights for Presentation

Fore the presentation, I will be highlighting the relationships between the loan amount and the three categorical variables of interest.
I chose findings based on the categorical variables as they seem to have the most impact on the loan amount compared to the numerical features of interest. I will highlight the effect of income range, isborrowerhomeowner, and income verifiable features have on the loan amount.
I will start by showing the distribution of the loan amount variable, followed by the credit score range variable. Afterwards, I will introduce each categorical variables. I will finish by using point plots for each categorical variable against the loan amount variable.
