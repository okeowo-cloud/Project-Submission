# Analyze Supermarket Data Across the Country - Company XYZ

## Description

Company XYZ owns a supermarket chain across the country. Each major branch located in Lagos, Abuja and Port Harcout recorded sales information for 3 months (Between January 2019 and March 2019), to help the company understand sales trends and determine its growth, as the rise of supermarkets competition is seen to increase.



# Project Steps

## Step 1 -  Loading the Dataset

Files (csv) containing sales record of each branches of company-xyz was loaded automatically from the directory and concatenated using the pd.concat function into a single dataframe.

## Step 2 - Data Exploration

The data was then explored to get basic information about the data such as:

* The Shape of dataframe using df.shape
* The Columns in dataframe using df.columns
* The statistical summary of quantitative variables in dataframe using df.describe()
* The presence of missing values using df.isnull() or df.notna()
* Other infomation about dataframe using df.info()

## Step 3 - Data Pre-processing

The Pre-processing task carried out in this project include:

* Formatting Date column to datetime datatype using pd.to_datetime()
* Extraction of Day, month and Year from the Date column and saving to new columns of Day, Month and Year respectively
* Formatting Time column to datetime datatype using pd.to_datetime()
* Extraction of Hour from Time column and saving to new Hour column 

## Step 4 -  Data Analysis

The analytic tasks carried out in this project include:

### TO DO A -

I determined the Unique hours of sales of company-xyz and the count (frequency) of this sales time using df.unique()

### TO DO B - 

I determined the list of items in all categorical columns such as: Invoice ID, Branch, City, Customer type, Gender, Product line and Payment using df.unique().tolist()

### TO DO C - 

I determined the Count of items in unique categorical columns using df.value_counts()

### TO DO D - 

I aggregated the dataframe by City and execute the Mean and sum function on it using df.groupby().mean() or df.groupby().sum()


### TO DO E - 

I splice the dataframe into two based on rating i.e. Rating <= 5 and Rating > 5. I grouped the dataframe by city and execute the mean and sum function on it.

I determined the City with the highest low rating i.e. Rating equal to and below 5
I determined the City with the highest high rating i.e. Rating above 5.
I determined the City withn the Overall mean and total rating from original dataframe


## Step 5 - Data Visualization

### TO DO A -

I plot a bar graph of City showing their :

* Total Gross Margin Percentage
* Total Gross Income
* Total Cost of goods sold (cogs)
* Total Rating

### TO DO B - 

* (a.) I determined the most used payment method by customers in branches of company-xyz
* (b.) I determined the most used branches of company-xyz or branch with the highest sales record
* (c.) I determined the count of the gender of customer types in company xyz
* (d.) I determined the count of customer types in branches of company-xyz
* (e.) I determined the count of customer gender  in all branches of company-xyz

### TO DO C - 

* (a.) I determined the highest and lowest product line sold by company-xyz
* (b.) I determined the Count of Product line sold in branches of company-xyz

### TO DO D - 

* I described the ratings of company-xyz using a Box plot

### TO DO E-

* I determined the effect of Gender on Productline sold by plotting Product line against Quantity and Hue it using Gender

### TO DO F -

* I determined the interaction between Unit Price and Quantity of goods sold by making a catplot of Product line per unit price and Product line per Quantity

### TO DO G-

* I determined the interaction between Gender and Unit Prices of Product line sold by making a line plot of Product line against Unit Price and hue by gender

### TO DO H-

* I determined the interaction between Gender and Quantity of Product line sold by making a line plot of Product line against Quantity and hue by gender

### TO DO I -

* I determined the Interaction between Productline per unit price and Productline per unit Quantity using a Violin plot

### TO DO J -

* I determined the Interaction between Productline per unit price and Productline per unit Quantity for Gender using a Violin plot


### TO DO K-

* I determined the Gross income by Productline in branches of company-xyz

### TO DO L -

* I determined the effect of customer type on the rating of branches of company-xyz

### TO DO M-

* I determined the relationship between Productline and Time of Purchase in branches of company-xyz

### TO DO N -

* I determined the relationship Between Hour of sales and Gross income of Branches of Company-xyz

## Step 6 - Insights

* The Unique sales hour of company-xyz are 10, 11, 12, 13, 14, 15, 16, 17, 18, 19 and 20.
* The Highest number of sales are recorded at Hour 10, 13, 16 and 19, with the most sales at hour 19.
* The City with the Highest Sales record is Lagos
* The customer type with the highest purchase record are the members
* The customer gender with the highest purchase record are the Females
* The females are the most customer type with membership status in company-xyz
* The males are the most Customer type without membership status i.e. Normal customer.
* The Most sold Productline are the Fashion Accessories, followed by Food and Beverages
* The Most used Payment method is the E-pay followed by cash then card being the least.
* Port Harcout City has the highest total Gross income, followed by Lagos and Abuja is the least.
* Lagos City has the Highest Gross margin Percentage
* Abuja has the highest low rating
* Port Harcout City has the Highest Overall Mean rating i.e. rating per customer
* Lagos City has the highest Overall total rating
* Port Harcout City has the highest cogs, followed by Lagos and Abujais the least
* Cash Payment is the most frequent payment method in Port Harcout City
* E-pay is the most frequent payment method in Lagos City
* Card Payment is the most frequent payment method in Abuja City
* Port Harcout City has the highest customer type with membership status
* Lagos City has the highest non-member customer type i.e. Normal customer
* The Females are the highest customer gender in Port Harcout City
* The Males are the highest customer gender in Lagos City
* The most sold productline in Port Harcout City is Food and Beverages, followed by Fashion accessories and its sales is higher than those of Lagos and Abuja
* The most sold Productline in Lagos is Home and Lifestyle, and Electronic accessories and its sales is higher than those of Port Harcout and Abuja
* The three most sold productline in Abuja are Sports and travel, Fashion accessories, and Health and Beauty.
* The Quantity of goods sold decreases with increasing Unit price of goods.
* The female customer purchased more Quantity of goods with lower unit price while the male customer purchased low quantity of goods with higher unit prices.
* Food and Beverages, Electronic accessories, Sports and travel, and Fashion accessories products contributed the largely to the gross income of Port Harcout City with Food and Beverages contributing the most.
* Health and Beauty, and Home and lifestyle products contributed the most to the gross income of Abuja City
* Health and Beauty Products contributed the least to the gross income of Lagos City
* The gross income of Port Harcout City is maximum between 18 - 20 Hour
* The gross income of Abuja City is maximum at 17 Hour
* The gross income of Lagos City is maximum at 19 Hour 



## Future Work

Future work will be to divided the dataframe into three parts based on hours: 

* df_early for sales between 10 - 13 Hour 
* df_mid for sales between 14-16 Hour
* df_late for sales between 17-20 Hour

All the Analysis carried out in this project will then be repeated for these three dataframes 

This will help to uncover various relationships already seen in this current project in a temporal manner


## Standout Section

The Major Standouts in this project include:

* TO DO A - I plotted a bar graph of City showing their : Total Gross Margin Percentage, Total Gross Income, Total Cost of goods sold (cogs),  Total Rating.

* TO DO M - I determined the relationship between Productline and Time of Purchase in branches of company-xyz

* TO DO N - I determined the relationship Between Hour of sales and Gross income of Branches of Company-xyz

* TO DO K - I determined the Gross income by Productline in branches of company-xyz

* TO DO L - I determined the effect of customer type on the rating of branches of company-xyz

* TO DO E - I splice the dataframe into two based on rating i.e. Rating <= 5 and Rating > 5. I aggregated the dataframe by city and execute the mean and sum function on it.

    * I determined the City with the highest low rating i.e. Rating equal to and below 5
    * I determined the City with the highest high rating i.e. Rating above 5.
    * I determined the City with the Overall Sum and mean rating 
