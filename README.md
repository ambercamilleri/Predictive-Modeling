# ##############################################################################
# Predictive Modeling Project: Predicting AirBnB Prices
### Authors: Amber Camilleri, Christopher Kreke, Yuke Liu, Rachel Meade, Jayant Raisinghani
#
# Please add comments to this file before uploading
################################################################################

### Meeting Notes: https://drive.google.com/file/d/1ZEV8YxGwl6d5pZQ77DXOnlIp6y0Cgoaj/view?usp=sharing
### Final Presentaion: https://drive.google.com/file/d/16qanBS7IXIgpPZNCSQ8VjEhaBff8fh6s/view?usp=sharing

### #############################################################################

### V2 Uploaded
Changes Include: 
- addition of "host_is_superhost","number_of_reviews","and "number_of_reviews_ltm" to variables
- fixed formatting of "price", "security_deposit", and "cleaning_fee" to be numeric, without commas or "$"
- added column at end that has ((price x4) + cleaning_fee)
- removed any lisings that have >14 day minimum_nights (the meeting mins say >13, but I don't think 13 v 14 makes much difference)
- I have NOT changed columns that are basically Y/N to be bianary, like "room_type", for example. 
- Also, it may be useful to note that in both this file and the original I uploaded I set the working directory to one of my local folders. You'll obviously need to change this to the location of where you have the csv data file saved. 

As you guys continue working on this, feel free to clean up and make changes to the code I wrote. I like doing this for the practice, but have little experience. I'm certain my code is clunky at best. 


### V3 Uploaded
Script to get fully cleaned data

### V4 Uploaded
Changes Include:
- No longer calulating 'four_nights_price'
- Dropped entries with 'price' > 500
- Formatted 'price' column to remove decimal places
- Drop 'id' and 'name' column
- Write 'clean_listings_price500' to csv

### New CSV File --> "clean_listings_price500" 
- converted some of the non-numeric variables into 0-1 / or dummy variables

### Airbnb_Linear_Regressions_P500
- Forward, Backward, and Stepwise Multiple Regressions
- Ridge & Lassso (not using some - 2, I think - non-numeric variables)
- Explore relationships by creating correlation table and linear regressions

### Airbnb_RF_Boosting: 
- Tried predicting with price > 500 but RMSE was coming out to be huge with all the tree techniques 
- Predicted for price < 500 and RMSE is coming ~77. 
- Tried with different depths, aplha values , sizes and important variables 
