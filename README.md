# Udacity project 3 - Data Visualization
`Explore`, `Explain`

<strong>Data set:</strong> prosperLoanData.csv<br>
<strong>Data set dictionary:</strong> <br>
- `Prosper Loan Data - Variable Definitions - Sheet1.csv`
- `Prosper Loan Data - Variable Definitions - Sheet1.pdf`

# Dataset
This [data set](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv) contains 113,937 loans with 81 variables on each
loan, including loan amount, borrower rate (or interest rate),
current loan status, borrower income, and many others.
This [data dictionary](https://www.google.com/url?q=https://docs.google.com/spreadsheet/ccc?key%3D0AllIqIyvWZdadDd5NTlqZ1pBMHlsUjdrOTZHaVBuSlE%26usp%3Dsharing&sa=D&ust=1554484977407000) explains the variables in the data set.
Our Exploration is on a subset of the variables. spcific to our visualization.
The analys is carrried out in the fashion
##### Introduction
- In this step, we introduce the dataset and give its basic information.
    
##### Preliminary Wrangling
- In this step, we perform the wrnagling steps
    - Gather
    - Assess
    - Clean
        - Define
        - Code
        - Test
        
##### Univariate, Bivariate, and Multivariate Data Exploration
- In this section we first perform univariate exploration and pick varibles of interest
- Next we perform bivarite exploration on the variables of interest
- finally, we expand our exploration of the visualizations.
- The variables of interest are split between categorical variables and Quantitative variables.
    - The categorical variablef of interest; `LoanStatus`, `Term`, `Occupation`, `EmploymentStatus`, `IncomeRange`, `LoanOriginatioQuarter`, `ListingCategory`, etc.. were chosen because of they are mostly within the purview of the loan applicant and are used to classify loan applicants, while,
    - The Quantitative variables of interest; `BorrowerAPR`, `DebtToIncomeRatio`, `LoanOriginalAmount`, `MonthlyLoanPayment`, etc.. were chosen mostly because they are components of our summary statistics.

# Summary of findings
### Overall Summary
#### Univariate exploration
1.  - `Default` loans account for `10.6%` of the loans.
    - `Completed` loans account for `33.7%` of the loans.
    - `Current` loan saccount for 49.3% of the loans.
2.  - California has the highest number of loan applicants with `Texas`, `Florida`, `NewYork`, etc. following suit.
3.  - Employed clients account for 60.1% of the total loan applicants, wit 23.8% working full-time.

4.  - Applicants earning `$(25k - 74999k)` account for `55.4%` while clients earning  `$(75k - 100k+)` account for 30% of the total.
5.  - Most loan are in the fourth and first quarter respectively.
6.  - Most loans were recorded in 2013 with a high of 34000 loans.
7.  - `Home Ownership (IsBorrowerHomeowner`) has no effect on `loan performance (LoanStatus`).
8.  - `Computer Programmer`, `Executives`, `Teachers`, etc.. are some the major loan applicants
9.  - `Debtconsolidation` accounts for most loan categories.
10. - The loans are najorly longterm with a significant portion having a span of three years.
11. - Loan Amounts are mostly in multiples of `$5000`.
12. - A significant portion of the loan payments fall below `$1000`.
13. - The BorrowerAPR for most loans falls between `0.15` to `0.3`.

#### Bivariate Exploration <br>
#### category vs category
1. - `IncomeRange` affects `LoanStatus`.
2. - `Homeownership` has no effect on `LoanStatus`.
3. - `CreditGrade` is a reflection of previous loan performance `(LoanStatus)`.
4. - `EmploymentStatus` has mild effect on `LoanStatus`.
5. - Loan `Term` has no effect on `LoanStatus`.
#### Numeric vs Category
6. - Despite the tendencies of current loans being `pastdue`, there is no clear statistics showing that `LoanOriginalAmount` has any pronounced effect on `LoanStatus`.
7. - `BorrowerAPR` has significant effect on `LoanStatus`.
#### numeric vs numeric
8. - `BorrowerAPR` decreases with an increase in `LoanOriginalAmount`.
   - `BorrowerAPR` and `LoanOriginalAmount` are negatively correlated.
   - Along the years, `Completed` loans have lower `BorrowerApr` amidst increasing `LoanOriginalAmount`.
   - `Canceled` loans are also characterised by high increasing `LoanOriginalAmount`s and deacreasing `BorrowerAPR`.
#### Multivariate exploration
1. - `MonthlyLoanPayment` and `LoanOriginalAmount` are positively correlated with completed loans hiving a higher correlation coeficient.
2. - Home owners have lower `BorrowerAPR` than those who do not own homes.
3. - Lower `BorrowerAPR` values are associated with better `CreditGrade`s.

- Some of these exploration will be used in the `Explanatory Eploration` precisely the Multivariate explorations

## Key insights for presentation
- For our summary visualizations, we chose bivariate and Multivariate explorations bacuse they capture multiple insights than univariate explorations.