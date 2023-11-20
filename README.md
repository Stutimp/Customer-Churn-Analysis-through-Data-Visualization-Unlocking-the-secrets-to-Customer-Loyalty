# Project-1
#First I imported all the relevant dependencies in the jupyter notebook.
#I made a path and made a copy of my original dataset,i.e, Telco_Customer_Churn and named the copied dataset as "Telco_Customer_Churn_copydataset.csv", in order to save my original dataset as it is and work with only the copy of it and finally I read the dataset with read_csv().
#I started with checking my dataset, all columns and rows and looked for any null, missing values.

# I checked the data types of my columns and seperated recognized my numerical and categorical columns in order to proceed my analysis.

#I converted the churn column, my dependent variable into numeric using mapping function and added additional column for it, so i can also do some meaningful calculations beside the original churn column which is categorical here.

# I started checking with my first independent factor , monthly charges and tried to find any connection with churn rate.

# I created histograms, swarm plots, box plots and even went little ahead later on and made some monthly charge bins in order to make deeper analysis.
#By creating bins for monthly charges I attempted to understand the churning behavior with different variable under certain monthly charge bin.
#I Grouped by "monthly_charge_bin" and calculating the mean of numeric columns then made derived some statistical analaysis.

# I created scatterplot, and also added linear regression equation and line to the plots.

#After some deeper evaluations with monthly charges, I moved on with some other relevant factors of the dataset, such as Gender, Streaming TV Services, Contract Catagories, Internet Service Categories, Senior Citizenship status, Tenure, and finally Total Charges.
# I created pie charts, histograms,  and also did some statistical calculations for these factors.

# calculated Corelation coefficient in relation to churn  variable and used pandas' describe() function to statistically summarize the several data frames. 

#I created box plots for 'total charges' column as well to find possible outliers (extreme values) in both churned and retained customers categories to understand the customer churning behavior.
#I made 2 sets of pwer point presentations (slides) here, one is for the record and one is for my on line class presentation.Both are the final slides , i just made one shorter for easier lookup.

# Finally I noted down some important insights and findings as a conclusion of this project towards the end.
# I used online pandas, matplotlib, and seaborns documentations sources as references to work on my codes, the links are , https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.describe.html, https://matplotlib.org/3.7.1/tutorials/introductory/quick_start.html
 and https://seaborn.pydata.org/generated/seaborn.scatterplot.html 
 
 #I also got valuable suggestions and dataset insights from my online tutor from bootcamp and my TAs at bootcamp.
 
 #Thankyou