## 	Investigating Customer Buying Patterns at Blackwell Electronics


* [Project Overview](#project-overview)
* [Business Problem](#business-problem)
* [Primary Questions](#primary-questions)
* [Objective](#objective)
* [Data Collection](#data-collection)
* [Data Preparation](#data-preparation)
* [Analytical Techniques](#analytical-techniques)
* [Exploratory Data Analysis](#exploratory-data-analysis)
* [Insights & Findings](#insights--findings)
* [Recommendations](#recommendations)
* [Limitations](#limitations)
* [Conclusion](#conclusion)
* [Next Steps](#next-steps)
* [References & Resources](#references--resources)






## Project Overview
This project focuses on analyzing customer buying patterns from Blackwell Electronics’ eCommerce and in-store transactions. Using the data provided, the goal is to identify spending behavior by region and explore the relationship between the number of items purchased and the amount spent. Additionally, we will explore demographic differences and online versus in-store purchasing behavior. The findings will inform future marketing strategies and site enhancements.

## Business Problem
## Primary Questions: 
1.	Do customers in different regions spend more per transaction? Which regions spend the most/least?
2.	Is there a relationship between the number of items purchased and the amount spent?
## Objective:
This project aims to uncover insights from the transaction data to guide decisions on eCommerce site enhancements, marketing strategies, and improve customer targeting based on buying patterns.
________________________________________
## Data Collection
•	Data Source: The data provided by Blackwell Electronics includes transaction details from both online and in-store sales.
•	Data Variables: 
1.	In-store (Purchase Mode): Indicates whether the transaction was made in-store (1) or online (0).
2.	Age: Customer’s age.
3.	Amount: The total transaction value.
4.	Items: Number of items purchased.
5.	Region: The region where the transaction occurred (1 = North, 2 = South, 3 = East, 4 = West).
________________________________________
## Data Preparation
•	Checking duplicate values 
•	Checking for missing values
•	Checking for outliers
•	Data Transformation:
o	Renamed columns for better clarity: "In-store" to "Purchase Mode" and "Region" to full names (e.g., North, South, etc.).
o	Converted categorical columns to appropriate data types (e.g., Purchase Mode and Region from numerical to categorical).
•	Data Cleaning:
o	Ensured consistency in the categorization of the "Region" and "Purchase Mode" columns.
o	Removed any inconsistencies or missing values in the data.
•	Data Binning:
o	Created an "Age Group" categorical variable to analyze age patterns more effectively.
________________________________________
## Analytical Techniques
•	Approach: This analysis employs exploratory data analysis (EDA) techniques to understand the relationships between variables and discover insights.
•	Tools & Technologies:
o	Python with Pandas and Matplotlib for data manipulation and visualization.
o	Scikit-learn for building machine learning models (Decision Tree, Random Forest, Gradient Boosting Classifier).
•	Statistical Methods:
o	Univariate Analysis: Basic analysis of the distribution of variables such as transaction count by region and spending amounts by region.
o	Bivariate Analysis: Examined relationships between spending amounts and number of items purchased, as well as the region and purchase mode.
•	Assumptions:
o	All data is assumed to be accurate and represents genuine customer behavior.
________________________________________
## Exploratory Data Analysis (EDA)
•	Univariate Analysis: 
o	Transactions by Region: The West region had the highest transaction volume, followed by South, East, and North regions (lowest).
•	Bivariate Analysis: 
o	Region vs. Purchase Mode: 
	North: No online purchases.
	South: Only online purchases.
	West: Equal in-store and online purchases.
	East: More in-store purchases than online.
o	Spending by Region: 
	West: Highest spending per transaction.
	South: Lowest spending per transaction.
o	Items vs. Amount Spent: 
	Items 2 and 8 had the highest amounts spent with relatively low variation.
________________________________________
## Insights & Findings
Findings: From the confusion matrix above, I observed that the model was not able to predict correctly at each point which might be as a result of the datatype used for the categorical variables eg. region and Purchase Channel which have numerical values. It might also be as a result of discretization.
•	Regional Spending Patterns: 
o	The West region spends the most per transaction, followed by the East and North regions, while the South region spends the least per transaction.
•	Number of Items vs. Amount Spent: 
o	There is a noticeable relationship between the number of items purchased and the total amount spent. Items with higher quantities purchased tend to correspond to higher amounts spent.
________________________________________
## Recommendations
•	Marketing & Sales Strategy: 
o	Focus targeted promotions or discounts on the South region to increase spending per transaction.
o	For the West region, where the highest spending is observed, create loyalty programs or upselling techniques to further increase transaction amounts.
•	Site Enhancements: 
o	Consider improving the online shopping experience in the North and East regions by promoting online shopping and analyzing why the North region is not participating in online sales.
________________________________________
## Limitations
•	Data Limitations: 
o	The dataset does not provide demographic information beyond age, which limits further in-depth analysis of other factors affecting purchasing behavior.
o	The data does not contain information about product categories or customer preferences, which could be valuable for segmenting customers.
•	Model Limitations: 
o	The models used (Decision Tree, Random Forest, Gradient Boosting) may not capture all complex relationships within the data, and more sophisticated techniques like neural networks could be explored in the future for better predictions.
________________________________________
## Conclusion
•	Key Findings: 
o	There are significant differences in spending patterns across regions, with the West region spending the most per transaction and the South the least.
o	The number of items purchased is positively correlated with the total amount spent.
## Next Steps: 
o	Further analysis could focus on understanding more granular customer demographics and preferences.
o	Future phases should explore predictive modeling to forecast purchasing behavior and optimize inventory or marketing efforts.
________________________________________
# References & Resources
•	Data provided by Blackwell Electronics.
•	Python libraries: Pandas, Matplotlib, Scikit-learn.
________________________________________

