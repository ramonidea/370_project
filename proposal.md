# What makes Kickstarter Campaign successful?

### INFO 370 Final Project
Tabitha Anderson, Autumn Derr, John Soter, Katie Clark, Ramon Qu

## Project Description

### Purpose

The main **purpose** of our research project is to **predict what makes a successful Kickstarter campaign**.
Also, we would like to look at the current crowd funding market in general, in order to evaluate the data. We would also like to look into what kind of campaign do people donate the most (e.g. board games, movies, apps, etc).  We would like to also try to make a model for predicting the success rate of campaigns during different time periods (e.g. would starting your campaign during the holiday season affect your chances of success?).

This is important as it could *help* let people who potentially want to do a Kickstarter know the best ways for achieving success. Also, sites such as Kickstarter and Indiegogo have become *immensely popular*. Being able to predict which projects are *likely* to succeed or fail can stop people from spending their money on a risky project. Since 2012, Kickstarter had over 400,000 campaigns and there have been more 3.9 billion dollars pledged to campaigns. Of that 3.9 billion dollars, 408 million dollars have been spent on unsuccessful campaigns [Kickstarter Statistics 2012-2018](https://www.statista.com/topics/2102/kickstarter/).

### Current Research Papers
When beginning to research the topic of determining why some kickstarter domains are *more* successful than others, we found that there were many people who had an interest in this topic as well. One of these pieces of [research](https://github.com/ktclark98/370_project/blob/master/paper/Crowdfunding_Success.pdf) attempted to find the best model to show why some projects perform better than others. This research was conducted by using a negative binomial distribution. Something that we found interesting about this specific experiment was how *easy* it was for them to get significant results. They only used three parameters with their model but were able to find that the success was affected by the *number* of projects previously run by the creator helps improve their experience to then run more successful campaigns and get more backers in the future. This is not something that we had previously discussed for some of our possible variables, but based on the success of this research, it seems like a promising direction to incorporate in our experiment.

Another piece of [research](https://github.com/ktclark98/370_project/blob/master/paper/Predicting_the_Success_of_Kickstarter_Campaigns.pdf) that we found also worked with finding what could make Kickstarter Campaigns more successful. This article had a key similarity with the previous article where they also found that there was a significant increase with their R-Squared value for their linear regression model when past successes were part of the equation. Some other significant variables that were found were the number of Facebook friends, number of perks, number of updates, and number of images. However, this research only has data that is present in *2017*. I believe that we can expand on this research with the dataset that we have that includes many years of data.

The last [research article](https://github.com/ktclark98/370_project/blob/master/paper/Show_me_the_money!_An_analysis_of_project_updates_during_crowdfunding_campaigns.pdf) that we found had a different focus than the other two articles. While it was still attempting to find what helps these campaigns be successful, there seemed to be a large emphasis on the amount of *updates* a Kickstarter campaign had. They looked specifically at the usage pattern of these updates and how different types of updates were associated with the *success* of a campaign. This was done by breaking apart the updates and analyzing them with decomposition based on punctuation.

Based on these three articles it can help us figure out how our research will fit into this domain. We believe that our research will fit in closer with the two first research articles. While the idea of the updates is interesting, it doesn't seem likely we will be able to come up with a way to categorize these updates based only on the text. This means that we will have to take some of these previous ideas and try to build on them to come up with the best model that we can.

### Hypothesis
- What categories, other attributes lead to a more successful kickstarter campaign?
- What are the qualities that make a bad campaign?
- Is it possible to predict what makes a campaign succeed or fail?

### Dataset(s)
We are looking at multiple crowdfunding site's project datasets, which contains their successful rate and other information.  
- [Kickstarter Projects dataset](https://webrobots.io/kickstarter-datasets/)
- [Indiegogo Data Set](https://webrobots.io/indiegogo-dataset/)
- [Kaggle Kickstarter Projects Dataset](https://www.kaggle.com/kemical/kickstarter-projects)
- [Indiegogo Kaggle proect Dataset](https://www.kaggle.com/kingburrito666/indiegogo-project-statistics)

Both of the datasets are scraped data from the websites, which is done by [Webrobots](https://webrobots.io/)

Both datasets contains 703k projects from Kickstarter and 600k Indiegogo projects.

### Statistical and Machine Learning Methods
- Because we have previous project data from both crowdfunding platforms, we are able to use supervised learning model to predict the successful rate for a new project.
- Because of the dataset is large enough, according to the [blog](https://www.datasciencecentral.com/profiles/blogs/which-machine-learning-algorithm-should-i-use),
- We can use classification models to see the attributes that successful projects share. May use KNN and other supervised learning model to predict the successful rate for a new project

### Target Audience
There are a couple audiences for this resource.

1. People interested in creating a successful Kickstarter/Indiegogo campaign.
2. People who want to know which Kickstarter campaigns are worth investing in. 

While each of these audiences would reap the benefits of knowing what makes a better campaign, we will primarily focus on those looking to fund their project ideas.

### Target Audience Questions
From this resource, those looking to make successful Kickstarter campaigns will understand what characteristics or combination of characteristics works best for Kickstarter campaigns. The data analysis that we will perform will help them build the most successful campaign for their product or idea. Knowing this information will help designers and innovators reach more people and garner a large support base, as well as help them fund a project.

## Technical Description

### Format
 We will use **Python Jupyter Notebook** to generate our report and visualize the graphs.

### Data Management Challenges
 The data set we got from Kaggle is massive, and it cannot be directly imported by Python. We may need to do some data cleaning before working on it.

### New Technical Skills
 - We may need to investigate other supervised learning which fits our problem domain more.
 - We need other techniques to clean our data sets.
 - We anticipate having to learn more skills, though currently it is hard to say what those will be. Our best guess is that it will focus on learning more skills relevant to machine learning with python packages and creating good in-depth visualizations to display our results.

### Conduct Analysis
 Currently, our modeling approach consists of applying the machine learning skills we learned in class in notebook 6. Specifically we will use the **sklearn** package. We will create both a decision tree model and K-nearest neighbors model. We might also do some logistic modeling and maybe some linear modeling, to have a second angle at which variables are most important to the success (or failure) of a kickstarter. Once we do these initial steps, we will see what are results are at that point and see if/what we want to do beyond the modeling we learned in class.

### Major challenges
One issue we might face is the task of analyzing two *different* sources of information for similar trends. Kickstarter and Indiegogo are similar in that they're both crowdfunding websites but *differ* in the types of projects that get listed on either website. For instance, Kickstarter is usually used to fund the creation of some kind of product. While this also occurs on Indiegogo, a lot of people use Indiegogo as a means to seek personal funding for activities such as trips or vacations. Because of this, it may be difficult to find a generalized model for both services that can accurately predict if a project is going to succeed or fail.

Another issue we might face is working with a dataset so *massive*. The Kickstarter dataset alone is close to 54 GB of data. So training off a dataset that large will take a lot of processing time. Combine that with the fact that we are also using the Indiegogo dataset and you're looking at even more processing time.

## Public Github Repository
-  https://github.com/ktclark98/370_project
