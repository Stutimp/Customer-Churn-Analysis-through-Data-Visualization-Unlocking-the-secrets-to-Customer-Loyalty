# Project-1
# Data Analysis on the Customers' Churning behavior of the tele communication Services

## Overview

### Purpose:
The purpose of this project is to find the answers of the following key questions:

- Does the high monthly rate and high total charges make more customers churn?

- Are there other factors in the dataset, such as Gender, Streaming TV availability, Senior Citizenship, contracts, and  Internet Services that have more vital connection with the churn?

## Data Sources:
This clean dataset with no null values, is collected from the GitHub page. The link is here posted: https://www.kaggle.com/datasets/blastchar/telco-customer-churn.
- Numerical columns in the dataset are: Senior Citizen, tenure, and Monthly Charges 
- Categorical columns: All other columns, including Total Charges, are listed as string/object data type. 


Steps I followed are: 

- First I imported all the relevant dependencies in the jupyter notebook.
- I made a path and made a copy of my original dataset,i.e, Telco_Customer_Churn and named the copied dataset as "Telco_Customer_Churn_copydataset.csv", in order to save my original dataset as it is and work with only the copy of it and finally I read the dataset with read_csv().
- I started with checking my dataset, all columns and rows and looked for any null, missing values.

- I checked the data types of my columns and seperated recognized my numerical and categorical columns in order to proceed my analysis.

- I converted the churn column, my dependent variable into numeric using mapping function and added additional column for it, so i can also do some meaningful calculations beside the original churn column which is categorical here.

 - I started checking with my first independent factor , monthly charges and tried to find any connection with churn rate.

- I created histograms, swarm plots, box plots and even went little ahead later on and made some monthly charge bins in order to make deeper analysis.
#By creating bins for monthly charges I attempted to understand the churning behavior with different variable under certain monthly charge bin.
#I Grouped by "monthly_charge_bin" and calculating the mean of numeric columns then made derived some statistical analaysis.

- I created scatterplot, and also added linear regression equation and line to the plots.

- After some deeper evaluations with monthly charges, I moved on with some other relevant factors of the dataset, such as Gender, Streaming TV Services, Contract Catagories, Internet Service Categories, Senior Citizenship status, Tenure, and finally Total Charges.
- I created pie charts, histograms,  and also did some statistical calculations for these factors.

- Theb calculated Corelation coefficient in relation to churn  variable and used pandas' describe() function to statistically summarize the several data frames. 

- I created box plots for 'total charges' column as well to find possible outliers (extreme values) in both churned and retained customers categories to understand the customer churning behavior.
- I made 2 sets of pwer point presentations (slides) here, one is for the record and one is for my on line class presentation.Both are the final slides , i just made one shorter for easier lookup.

- Finally I noted down some important insights and findings as a conclusion of this project towards the end.
-  I used online pandas, matplotlib, and seaborns documentations sources as references to work on my codes, the links are , https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.describe.html, https://matplotlib.org/3.7.1/tutorials/introductory/quick_start.html
 and https://seaborn.pydata.org/generated/seaborn.scatterplot.html 


## Observations and suggestions

1. With respect to "Monthly charges“, there is a weak positive linear relationship (0.193) between monthly charges and churn rate. Also, the R-squared value of (approx.) 0.212 indicates the strength of the relationship; it would also be essential to consider the p-value associated with the regression analysis to understand whether the observed relationship is statistically significant. 
 Suggestions: There could be other factors influencing churn that are not included in the model. These might include customer service quality, contract terms, competitive offers, individual customer preferences, and market conditions. 

2. With respect to the “Internet Services” category, Fiber Optic has the highest churn rate, i.e., 42%.  suggesting issues around fiber optic services. The provider could improve fiber optic performance and customer satisfaction to reduce churn. 
 Suggestions: Improving fiber optic satisfaction and analyzing the root causes of dissatisfaction among fiber optic customers could reveal ways to improve retention.


3. With respect to “Contract” categories, approx. 42.71% of customers with a month-to-month contract have churned,  compared to (one year and two years), with the two-year contract holders being the least likely to churn(2.83%). 

Suggestions:  The highest month-to-month churn rate could reflect the lowest commitment level, lower satisfaction, end of promotions and trial periods of the services, life changes, etc. Customized price levels ensuring higher quality ensuring customer satisfaction may help businesses retain more customers. 

4. With respect to “Total Charges:” The significant presence of outliers among churned customers suggests that while the median total charge is lower, several churned customers still have very high total charges. The more consistent range of total charges among retained customers could indicate that customers within a specific spending range are more likely to stay.

Suggestions: The company might want to investigate why customers with high total charges are leaving and address those reasons to improve retention.

5. With Respect to “Senior Citizen”: The churn rate is almost double for senior citizens versus non-seniors (41.68% >23.60%) even though seniors are only 16.2% of the total customers in the dataset. 
Suggestions: The smaller number of senior citizens in the dataset could mean we didn’t collect enough data from the aging population. At the same time, their higher churning rate suggests that they may need additional retention efforts, special offers, or customized services to reduce their churn rate.


### Conclusion

In conclusion, different variables undoubtedly have marginal effects on our variable “Churn.” However, it is also crucial to acknowledge that the interactions between these variables can influence churn in reality.   
 
 
 
 - I also got valuable suggestions and dataset insights from my online tutor from bootcamp and my TAs at bootcamp.
 
 Thank you!

 Author

 Stuti Poudel