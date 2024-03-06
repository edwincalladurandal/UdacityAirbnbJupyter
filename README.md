### Readme Udacity Project Airbnb
# Author: Edwin Calla Durandal
# Year: 2024

## Introduction
You will fine here the motivation for this project with a small description of the developing process, as well as a summary of the results of the analysis and basic acknowledments. We want to motivate to you to continue digging in the topic and data. 

We are going to develop an analysis using the open access data of Airbnb for Boston. We have 3 different files, being: calendar, listings and reviews. In all these files we have to do some cleaning, the idea and the challenge here is to not use any machine learning algorithm and make sense of the data that we received, considering the actual market.  

In straigth forward words, the goal is to analyse if it is interesting to get started or not in this business market. 

## Analysis 
We are going to present and share the personal point of view of the possibilities with the data that we have to work, so in this part we are going to present each dataset and explain a couple of possibilites for each, we encourage you to see more alternatives: 

*Calendar* 
Four columns containing _listingid_, _date_, _available_ and _price_ 
* _date_ we can take advantage of it because with this we can know how many days per month it was occupied, this is going to relate the columns _date_ with _available_, of course going deeper this is related with high or low seasons, that for sure is going to have an impact on the prices 
* talking about prices, we can see the _price_ variable to, then inside this CSV we can relate if the _price_ have something to see with the _available_
* _listing_id_ is the one that show to us the different alternatives that the guests have in Boston, from single rooms to complete houses or hotel rooms, this is a interesting thing when we relate with the information of the other dataframes

*List* 
Multiple columns, total of 95 including different kind of information like _id_, _listing_url_, _reviews_per_month_ etc... here we have to be careful with the NaN and the "none" values. We could consider the next bulletpoints to analyse: 
* we know here how many houses we have to rent, this is going to be related with the calendar
* here we should look for more information that could be useful for us because we have 95 columns of info
* we can consider how many information is shared from the owner and if that reflects how many clients take the offer
It is important to consider that it is not limitative and that if you put this dataframe togheter to the other ones, it is really usefull. The idea for the information presented in this document is how you can get started in this business market and if it is atractive. 

*Review* 
Here we have sixs columns containing _listing_id_, _id_, _date_, _reviewer_id_, _reviewer_name_ and _comments_.
* here we have how the _comments_ of the houses, then this is from the _reviewer_id_ that can give us an idea if the _comments_ help to the _id_ to have more entries
* we can see when they give a _comments_ intersecting the information with when they were in the room _date_ of the reservation
* Interesting to analyse why people did not put a _comments_ if its realeted with the expierence with the host or the place

We have two of each dataframe, then we could concentrate in analyzing the way of thinking on the people that rent! In other words, what they look for renting a place! In general senses could be the price and the reviews for example, we motivate to you digging in! 

## Questions
We are going to analize each file that we have to see after what we can do between them, once again, you are going to find all this on the Jupyter Notebook with their respective comments. The questions are as follows: 

* What is the information that the hosts do not usually put?
* Where is the location (zip code) with higher prices?
* Is it interesting to enter to the business of renting houses?

In the Jupyter Notebook you will find the codes with their respective comments and the images that helps you to analyse at a glance. 

## Motivation
We want to motivate to you to continue analyzing the data, so we are going to share some of the interesting values to look inside of the Dataframes LIST, REVIEW and CALENDAR:  
# List
* number_of_reviews
* review_scores_rating
* cancellation_policy
* host_identity_verified

# Review 
* listing_id
* id
* date
* comments

# Calendar
* listing_id
* date
* available 

Mergging this data, you should be able of finding more interesting insides. 

## Develop
The develop of the code it was following the simple steps of the great course in Udacity, Nano Degree in Data Science. They are the following: 
* Select a dataset
* Elaborate 3 questions related to the business data 
* Gather necessary data to answer your questions
* Handle categorical and missing data
* Provide insight the methods you chose and why you chose them
* Provide a clear connection between your business questions and how the data answers them
* Create Github repository
* Create a blog post

We want to emphasis that you have to be careful when you are elaborating the questions, you have much data to make some sense, so first look at the raw data and see what path you want to take and why. After you start the process, consider that the data could be 'dirty', then you should do a proper clean or convertion of the data to different formats, be conscious about it ;) 

## Comments
It was a fun job to do, if you can take the time to analyse deeply, you will understand much better why Airbnb works the way it works ;) good luck! And share with us your findings! Lets talk about business! 

## Libraries
It is necessary to use the proper libraries at the beggining of our code. You are going to see them with their proper info in the Jupyter Notebook. 

They are: 
* Numpy -> Fundamental library for scientific computing in Python
* Pandas -> Powerful library for data manipulation and analysis
* Matplotlib -> Plotting library that enables you to create a wide variety of static, animated, and interactive visualizations in Python
* Scikit-learn -> Popular machine learning library in Python 

## Acknowledgement 
For the development of the present project it was used different information and knowledge, so we would like to acknowledge to:
* Udacity for elaborating this practical course and the reviewers/professors behind everything
* Airbnb for giving an open-source data set
* Kaggle for offering a detailed information about the data set that helped to analyze beforehand
* All the people posting their own bugs and expiriences in StackOverflow, Medium or GitHub 

## Github Repository
https://github.com/edwincalladurandal/UdacityAirbnbJupyter.git

The files that you are going to find are:
* README.md all the basic information for a better understanding of the project
* FINALPROJECTAIRBNB.ipynb this is the Python code with a Jupyter Notebook view for easy access and understanding
* .GITIGNORE this is just for our use with GIT, you can ignore it 

## Blog
https://medium.com/@edwin.calla/blog-udacity-project-airbnb-424b36370575

Here you will find a summary of the results of the analysis, we invite you to go and read it! Of course if you want to participate with some comments, they are more than welcome! As a brief glance of the results, we can say that it is a fancy business to enter, if you have the interest joing this business, we recommend to you e-visit a couple of residences and if you have the chance to rent one fancy and one cheap, this could give you good parameters for understanding where you want to be. Good luck! 