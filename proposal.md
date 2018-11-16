# What makes Kickstarter Campaign successful?

### INFO 370 Final Project
Tabitha Anderson, Autumn Derr, John Soter, Katie Clark, Ramon Qu

## Project Description

### Purpose
The main **purpose** of our research project is to **predict what makes a successful kickstarter campaign**.
Also, we would like to look at the current kickstarter and other crowd funding market, in order to evaluate the data. We would also look into what kind of campaign does people donate the most.  We would try to make a model for predicting campaign successful rate in different time period. .............(Add why it is important)
### Current Research Papers
When beginning to research the topic of determing why some kickstarter domains are more successful than others, we found that there were many people who had an interest in this topic as well. One of these pieces of [research](https://github.com/ktclark98/370_project/blob/master/paper/Crowdfunding_Success.pdf) attempted to find the best model to show why some projects perform better than others. This research was conducted by using a negative binomial distribution. Something that we found interesting about this specific experiment was how easy it was for them to get significant results. They only used three parameters with their model but were able to find that the success was affected by the number of projects previously run by the creator helps improve their experience to then run more successful campaigns and get more backers in the future. This is not something that we had previously discussed for some of our possible variables, but based on the success of this research, it seems like a promising direction to incorporate in our experiment.

Another piece of [research](https://github.com/ktclark98/370_project/blob/master/paper/Predicting_the_Success_of_Kickstarter_Campaigns.pdf) that we found also worked with finding what could make Kickstarter Campaigns more successful. This article had a key similarity with the previous article where they also found that there was a significant increase with their R-Squared value for their linear regression model when past successes were part of the equation. Some other significant variables that were found was number of Facebook friends, number of perks, number of updates, and number of images. However, this research only has data that is present in 2017. I believe that we can expand on this research with the dataset that we have that includes many years of data.

The last [research article](https://github.com/ktclark98/370_project/blob/master/paper/Show_me_the_money!_An_analysis_of_project_updates_during_crowdfunding_campaigns.pdf) that we found had a different focus than the other two articles. While it was still attempting to find what helps these campaigns be successful, there seemed to be a large empahasis on the amount of updates a kickstarter campaign had. They looked specifically at the what the usage pattern of these updates were and how different types of updates were associated with the success of a campaign. This was done by breaking a part the updates, and analyzing them with decomposition based on punctuation. 

Based on these three articles it can help us figure out how our research will fit into this domain. We believe that our research will fit in closer with the two first research articles. While the idea of the updates is interesting, it doesn't seem likely we will be able to come up with a way to categorize these updates based only on the text. This means that we will have to take some of these previous ideas and try to build on them to come up with the best model that we can.

### Hypothesis
- What categories, other attributes lead to a more successful kickstarter campaign?
- What are the qualities that make a bad campaign?

### Dataset(s)
We are looking at multiple crowdfunding site's project datasets, which contains their successful rate and other information.  
- [Kaggle Kickstarter-projects dataset](https://webrobots.io/kickstarter-datasets/)
- [Indiegogo Data Set](https://webrobots.io/indiegogo-dataset/)

Both of the data sets are scraped data from the websites, which is done by [Webrobots](https://webrobots.io/)

Both datasets contains 703k projects from Kickstarter and 600k Indiegogo projects.

### Statistical and Machine Learning Methods
- Because we have previous project data from both crowdfunding platforms, we are able to use supervised learning model to predict the successful rate for a new project. For example, Random Forest Model, K Nearest Neighborhood, Cluster models,
- Because of the dataset is large enough, according to the [blog](https://www.datasciencecentral.com/profiles/blogs/which-machine-learning-algorithm-should-i-use), we can use classification models to see the attributes that successful projects share.

### Target Audience
There are a couple audiences for this resource. For example, people looking to crowdsource money for their cool project ideas, the funders of the project that want to get their reward from donating to a successful campaign. While each of these audiences would reap the benefits of knowing what makes a better campaign, we will primarily focus on those looking to fund their project ideas.

### Target Audience Questions
From this resource, those looking to make successful Kickstarter campaigns will understand what characteristics or combination of characteristics works the best for Kickstarter campaigns. The data analysis that we will perform will help them build the most successful campaign for their product or idea. Knowing this information will help designers and innovators reach more people and garner a large support base, as well as help them fund a project.


## Technical Description

### Format
 We will use **Python Jupyter Notebook** to generate our report and visualize the graphs.

### Data Management Challenges
 - The data set we got from the Kaggle is massive, and it cannot directly imported by python. We may need to do some data cleaning before working on it.
 - The important features for different projects in different categories are different, which we may have to do analysis on different categories of projects to make the model better.
 - In some of the columns, they have categorical data, which we need to convert to numerical for future prediction.

### New Technical Skills
 - We may need to investigate other supervised learning which fits our problem domain more.
 - We need other techniques to clean our data sets.
 - We anticipate having to learn more skills, though currently it is hard to say what those will be. Our best guess is that it will focus on learning more skills relevant to machine learning with python packages and creating good in-depth visualizations to display our results.

### Conduct Analysis
 Currently, our modeling approach consists of applying the machine learning skills we learned in class in notebook 6. We might also do some logistic modeling and maybe some linear modeling, to have a second angle at which variables are most important to the success (or failure) of a kickstarter. Once we do these initial steps, we will see what are results are at that point and see if/what we want to do beyond the modeling we learned in class.

### Major challenges
 What major challenges do you anticipate?


## Public Github Repository
-  https://github.com/ktclark98/370_project
