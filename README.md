# Udacity Starbucks Capstone Challenge
Capstone project Starbucks <br>
Udacity Nanodegree: Date Science

# Objective
In this project I try mo improve the advertisement strategy for Starbucks. <br>
To be succesful on this task I will mainly focus on the following five quesitons:
* What are the most predictive features or parameters for a completed offer
* What are the relations between the customer age, income and offer completion rate?
* Is the customer gender important for the offer completion rate?
* What is the most important channel for completing an offer?
* Is there any correlation between the offer types and offer completion rate?

# Procedure
I will proceed the following steps to answer the above mentioned questions and successfully complete this project:
* Data wrangling <br>
The Data wrangling chapter consists of multiple steps, namely: 'gathering data', 'assesing data' and 'cleaning data'. This is about loading and analyzing the input data sets, as well as cleaning the data that they can be used for further investigations. At the end I will merge the data frames to have one complete cleaned data frame which will be saved. In this way all the cleaning steps do not need to be repeated if one wants to analyze the data later on. 
* Exploratory data analysis <br>
The exploratory data analysis is about the analysis and visualization of the data. First of all, on gets a deeper feeling of the data, prepares first insights and if possible also answers the first questions from the problem set. 
* Machine Learning approche for recommendations <br>
After the data analysis, a chapter will present a machine learning approche for recommentations. First of all three different machine learning models will be used with training and test data, best best predicting model will be improved and used to predict the most predictive features on which Starbucks can then focus. 
* Recommendation <br>
The last section will summarize the results and give some recommendations for Starbucks advertisement campaign.

# Libraries
The code is written in Python3 and following python libraries are used within the project:
* pandas
* numpy
* math
* json
* time
* matplotlib
* seaborn
* sklearn


# Dataset
The simulated dataset has been provided by Starbucks and Udacity. 
It contains the follwing files:
* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed


# Results
* The data investigation should that the completion rate increased with customer age. In addition, if one gets the customer to view the offer, the completion rate is between 60% and 80% for users between around 40 years and 95 years.
* The income has a similar behaviour as the age. The success or completion rate is increasing linearly with the income. Starting from an income of around $35,000 and a completion rate of 50% up to a completion rate of about 90% for registered customers with an income of more than $100,000.
* Looking at the registered customers who completed all offers, it is obvious that the percentage of the female registered customers completing all offers increases compared to the total gender distribution. <br>
Therefore on this first look it could be that females are more likely to complete an offer than males.
* The received completion rate of the completed offer / received offer (blue in the above plot) is more or less equal through all advertisement channels, but if the offer has been viewed, the highest completion rate is visible for the ‘web’ channel with an increase of about 25%, followed by ‘email’ with an increase of about 20%.
* Discount offers which have been viewed are most likely to be completed. The decrease steps from the received to the viewed and completed bogo offers are pretty similar leaving the discount offer the most often completed one.
* The machine learning approche identified the five most predictive feaures which are income and the age with a hugh distance to the next important features, duration and difficulty. The fifth most important feature is the gender male.

Looking at these results, I would recommend Starbucks to focus on the age, income and gender of the customer and taking into account the difficulty and duration as well as the advertising channel of the offers. So overall the best rate for completing all offers are given for an elder female customer with a high income of at least $80,000. The offer should be a discount and distributed via web, email or mobile (in this order).


# Acknowledgements
I want to thank Udacity and Starbucks providing the simulated dataset. <br>
My results are summarized on a blog post which can be found here: <br>
https://jklinder.medium.com/how-to-improve-the-advertisement-campaign-for-starbucks-bf71fe6afb2a
