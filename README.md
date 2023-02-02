# Loan_Approval
### Required Tools

Jupyter Notebook

Excel

PDF Reader

### Overview
The original task was to use two data set types one structured and one unstructured. The structured data set was from lendingtree.com obtained from Kaggle, it consisted of banking information on past loans and showed if a borrower had paid the loan back in full or defaulted on the loan.  There were many other types of information such as fico scores, annual income, and debt-to-income ratio to name a few. This data was used to gain insight into how these different variables change if a borrower pays back a loan or defaults and then using machine learning predict if a potential borrower would default on a loan or not.  Upon inspection of the data set it was concluded that small businesses loans had a much higher rate of defaulting.
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
The loans were grouped into paid and not paid and the percentages of each was examined this showed that while most loan types made up similar percentages of each (example: around 40% of both paid and defaulted loans are due to debt consolidation) small business loans make up 5.5% of the paid in full loans and 11% of the defaulted loans. 

![image](https://user-images.githubusercontent.com/118774600/212776674-f1d09d96-130e-4bb5-b24d-9c0834a70e6f.png)

### Scrapping and MongoDB

Tweets were scrapped out of twitter using snscrape and placed into a list of dictionaries, one tweet per dictionary, these were then saved into a mongo data base so the same tweets could be used for the entire process.

### Insights
Similar to how the information about the small business loans were grouped and aggregated to find how each percentage of the total the loan types made up; the data was separated into different groupings for many of the questions proposed at the beginning.  These findings were graphed for easy understanding and a few results are shown below.  This process was also done strictly on small business loans to see how each variable changes from all loan types vs. just small business loans.

![image](https://user-images.githubusercontent.com/118774600/212777428-1fc9033d-4a7c-4293-b683-ed6567ac503d.png)

![image](https://user-images.githubusercontent.com/118774600/212777453-c2d20c9b-915b-47df-b7ca-f2345a635c0d.png)

![image](https://user-images.githubusercontent.com/118774600/212777493-17090c4e-6695-417d-b91c-adc5662fb637.png)

![image](https://user-images.githubusercontent.com/118774600/212777516-725500ee-acce-406a-96a9-ac7bd0704f67.png)

### Using regular expression on tweets
Phrases were placed into a regular expression and used to search through tweets to see if tweets could be found that would indicate a business is a higher risk.  Dunkin Donuts and Starbucks were used at first and now tweets were found as an example of a business that would be a high risk a bankrupt company (toys-R-us) was used and many tweets were able to be pulled out and identified as cause for concern.
### Machine Learning
The data was split 80/20 for training and testing.  Decision tree, Naive Bayes, SVM, and Random Forest were used to predict if the borrower would default or pay back the loan.  The results of Accuracy, Precision, and Recall were graphed alongside the Original lendingtree.com percentage of loans being paid back or defaulting. 

![image](https://user-images.githubusercontent.com/118774600/212778414-7106a5da-d6aa-4dd6-b810-f84beca5e691.png)

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

### Report
The report goes into more detail showing how the coding was preformed and it is explained along with further insights not shown in this readme.  It also contains a sentiment analysis.

