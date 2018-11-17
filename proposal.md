# What makes Kickstarter Campaign successful?

### INFO 370 Final Project
Tabitha Anderson, Autumn Derr, John Soter, Katie Clark, Ramon Qu

## Project Description

### Purpose
The main **purpose** of our research project is to **predict what makes a successful Kickstarter campaign**.
Also, we would like to look at the current Kickstarter and other crowd funding market, in order to evaluate the data. We would also look into what kind of campaign does people donate the most.  We would try to make a model for predicting campaign successful rate in different time period.

This project is important because crowdfunding sites such as Kickstarter and Indiegogo have become immensely popular. Since 2012, Kicksstarter had over 400,000 campaigns and there have been more 3.9 billion dollars pledged to campaigns. Of that 3.9 billion dollars, 408 million dollars have been spent on unsuccessful campaigns [Kickstarter Statistics 2012-2018](https://www.statista.com/topics/2102/kickstarter/). That's a lot of money and this isn't money coming from a venture capitalist, this is money coming from your average citizen. If a project fails, you don't get your money back. If we can figure out a way to predict which campaigns are most likely to be successful, then it could be used as a tool to see which projects deserve funding and which do not.

### Current Research Papers
The broader problem domain is that **BROADER PROBLOEM DOMAIN**  ....
What kind of research paper in this domain. **Cite three paper here**

### Hypothesis
- What categories, other attributes lead to a more successful kickstarter campaign?
- What are the qualities that make a bad campaign?
- Is it possible to predict what makes a campaign succeed or fail?

### Dataset(s)
We are looking at multiple crowdfunding site's project datasets, which contains their successful rate and other information.  
- [Kaggle Kickstarter-projects dataset](https://webrobots.io/kickstarter-datasets/)
- [Indiegogo Data Set](https://webrobots.io/indiegogo-dataset/)

Both of the data sets are scraped data from the websites, which is done by [Webrobots](https://webrobots.io/)

Both datasets contains 703k projects from Kickstarter and 600k Indiegogo projects.

### Statistical and Machine Learning Methods
- Because we have previous project data from both crowdfunding platforms, we are able to use supervised learning model to predict the successful rate for a new project.
- Because of the dataset is large enough, according to the [blog](https://www.datasciencecentral.com/profiles/blogs/which-machine-learning-algorithm-should-i-use),
- We can use classification models to see the attributes that successful projects share. May use KNN and other supervised learning model to predict the successful rate for a new project

### Target Audience
There are a couple audiences for this resource. For example, people looking to crowdsource money for their cool project ideas, the funders of the project that want to get their reward from donating to a successful campaign. While each of these audiences would reap the benefits of knowing what makes a better campaign, we will primarily focus on those looking to fund their project ideas.

### Target Audience Questions
From this resource, those looking to make successful Kickstarter campaigns will understand what characteristics or combination of characteristics works the best for Kickstarter campaigns. The data analysis that we will perform will help them build the most successful campaign for their product or idea. Knowing this information will help designers and innovators reach more people and garner a large support base, as well as help them fund a project.


## Technical Description

### Format
 We will use **Python Jupyter Notebook** to generate our report and visualize the graphs.

### Data Management Challenges
 The data set we got from the Kaggle is massive, and it cannot directly imported by python. We may need to do some data cleaning before working on it.

### New Technical Skills
 - We may need to investigate other supervised learning which fits our problem domain more.
 - We need other techniques to clean our data sets.
 - We anticipate having to learn more skills, though currently it is hard to say what those will be. Our best guess is that it will focus on learning more skills relevant to machine learning with python packages and creating good in-depth visualizations to display our results.

### Conduct Analysis
 Currently, our modeling approach consists of applying the machine learning skills we learned in class in notebook 6. We might also do some logistic modeling and maybe some linear modeling, to have a second angle at which variables are most important to the success (or failure) of a kickstarter. Once we do these initial steps, we will see what are results are at that point and see if/what we want to do beyond the modeling we learned in class.

### Major challenges
One issue we might face is the task of analyzing two different sources of information for similar trends. Kickstarter and Indiegogo are similar in that they're both crowdfunding websites but differ in the types of projects that get listed on either website. For instance, kickstarter is usually used to fund the creation of some kind of product. While this also occurs on Indiegogo, a lot of people use Indiegogo as a means to seek personal funding for activities such as trips or vacations. Because of this, it may be difficult to find a generalized model for both services that can accurately predict if a project is going to succeed or fail.



## Public Github Repository
-  https://github.com/ktclark98/370_project
