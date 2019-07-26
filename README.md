# ##############################################################################
# Predictive Modeling Project: Predicting AirBnB Prices
# Meeting Notes: https://docs.google.com/document/d/13sGsI9dkq4WxyQCRV87Vu5aBqmBYANkO341UxVx4Sco/edit
# 
# Please add comments to this file before uploading
################################################################################

Authors: Amber Camilleri, Christopher Kreke, Yuke Liu, Rachel Meade, Jayant Raisinghani

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
