# Loan_Approval
### Overview
The original task was to use two data set types one structured and one unstructured. The structured data set was from lendingtree.com obtained from kaggle, it consisted of banking information on past loans and showed if a borrower had paid the loan back in full or defaulted on the loan.  There were many other types of information such as fico scores, annual income, and debt-to-income ratio to name a few. This data was used to gain insight into how these different variables change if a borrower pays back a loan or defaults and then using machine learning predict if a potential borrower would default on a loan or not.  Upon inspection of the data set it was concluded that small businesses loans had a much higher rate of defaulting.
The unstructured data was tweets obtained about different businesses, to use regular expressions and create a way to determine if the small business held high risk based on what customers were saying about them.  These tweets were scrapped and placed into a mongo data base. 

### Questions
1. How does the average monthly amount due change in loans that were paid back vs loans 
that were not paid?
2. Does the purpose of the loan change the rate of being paid back or not?
3. A. Does annual income change the percentage of loans being paid back?
B. *What annual income ranges produces the least amount of defaulted small business 
loans?
4. A. Does more debt-to-income ratio change the percentage of loans being paid back?
B. * How does debt-to-income ratio change with small business loans?
5. A. How does fico credit score change the percentage of loans being paid vs not?
B. What fico credit rating range produces the least amount of defaulted small business 
loans?
6. Can sentiment analysis be used to increase knowledge and predict if a small business 
loan will default?
7. Can regular expressions be used to increase knowledge and predict if a small business 
loan will default?
8. Can machine learning provide a way to predict if an applicant will default on a loan?
9. Was anything found that significantly increase the chance that a small business loan 
does not default?
### Increased risk of small business loans

### Scrapping and MongoDB
### Insights
### Using regular expression on tweets
### Machine Learning
### Results (Answers)
1. How does the average monthly amount due change in loans that were paid back vs loans 
that were not paid?

• The monthly amount due is higher for defaulted loans than loans paid in full. The 
amount is about $33. Yet we see that the mean is much higher than the median 
meaning there is outliers on the large side for both.

2. Does the purpose of the loan change the rate of being paid back or not?

• Small business loans have a higher percentage of defaults compared to other loan 
types.

3. A. Does annual income change the percentage of loans being paid back?

• As annual income increases the rate of defaulting decreases. Except when looking at 
excessing of $200,000 income which can be contributed to small business loans to 
those individuals.

B. What annual income ranges produces the least amount of defaulted small business 
loans?

• Small business loans for income under $200,000 remains at smaller similar levels 
only increasing dramatically over the $200,000 income amount.

4. A. Does more debt-to-income ratio change the percentage of loans being paid back?

• As the debt-to-income increases so does the chance the loan will be defaulted

B.  How does debt-to-income ratio change with small business loans?

• It simply become more severe. The number of defaults is more and increase with 
debt-to-income at a higher rate.

5. A. How does fico credit score change the percentage of loans being paid vs not?

• As the fico credit score increases the percentage of loans defaulted drops.

B. What fico credit rating range produces the least amount of defaulted small business 
loans?

• As the fico credit score increases the percentage of loans defaulting drops. The first 
two groupings (699 and below and 700-799) have a much higher defaulting rate in 
small business loans compared to all loans. Best range is above 800.

6. Can sentiment analysis be used to increase knowledge and predict if a small business 
loan will default?

• While we did get an overall score for the brands, the scores were not a real 
representation of the brands themselves. A more specific sentiment analysis looking 
for specific words is needed to get a better sentiment score that represents what we 
are looking for.

7. Can regular expressions be used to increase knowledge and predict if a small business 
loan will default?

• Yes, using regular expressions allows for tweets of interest (indicating higher risk of 
defaulting) to be removed and displayed.

8. Can machine learning provide a way to predict if an applicant will default on a loan?

• Machine learning can be a powerful tool to help predict if a person will default on a 
loan or not.

9. Was anything found that significantly increase the chance that a small business loan 
does not default?

• Yes, Fico credit score, Debt-to-income ratio and regular expressions being used on 
tweets about the business in question can help identify if a small business is a greater 
risk of defaulting. Also, the income of the potential borrower can indicate that a 
closer look at them may be required. 

### Paper
