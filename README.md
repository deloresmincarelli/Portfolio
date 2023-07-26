## Delores Mincarelli Datascience Portfolio

## Welcome!  Let's begin with introductions: 
I'm a data sleuth.  
<br> To me, there is nothing more exciting than cracking open a new dataset. 

For years, I have rolled up my sleeves to help clinicians and managers make better decisions backed by sound data analysis. This required a deep - dive into their business, learning about their problems and concerns, and then being a professional sleuth to find and curate the data to underpin the analytics. 

I love using data-for-good. 

I like being involved end-to-end .. no need to throw a specification over the wall to me! I work side by side with customers in an iterative and layered approach so we have frequent checks and an evolution of the end result.

But one of the most important characteristics I bring is humility and passion for learning; I know how much I don't know. I'm **committed** to learning from others and sharing what I know to continually raise the bar for the organization.


## I'm driven by a strong sense of purpose:
![](https://github.com/deloresmincarelli/Portfolio/blob/main/images/PersonalMission.jpg)

## Now that you know who I am, let me show you what I can do:

## Project : Generating Synthetic Data
Wait .. I thought we were in the age of "big data"... why do we want to synthetically create more?
<br> Synthetic data is useful to complement existing data for "edge" cases, amplifying minority data, or even a way to circumvent using sensitive & protected information (like medical patient information).  Further, getting "real" data can be expensive especially in cases where you need to ruin what you are studying so you can get data before failure.  
<br> In this example, I used the Synthetic Data Vault (SDV), which is a Python library designed to be a one-stop shop for creating tabular synthetic data.
The SDV offers multiple machine learning models -- ranging from classical statistical methods (Copulas) to deep learning methods (GANs). 
It can generate data for single tables, multiple connected tables or sequential tables.
<br> This project is a proof-of-concept to get familiar with generating synthetic data.  
<br> Tools: Python - using Synthetic Data Vault
Example where SDV does a good job |  Example where SDV did not do a good job
:---------------------------------------------:|:-------------------------:
![](https://github.com/deloresmincarelli/Portfolio/blob/main/images/synthetic_data.jpg)  |  ![](https://github.com/deloresmincarelli/Portfolio/blob/main/images/synthetic_data2.jpg)

<br> [The details](https://htmlpreview.github.io/?https://github.com/deloresmincarelli/SyntheticData/blob/main/syndata_jetengine_singletable.html)


## Project :  Predicting Jet Engine Failure
<img src="https://github.com/deloresmincarelli/Portfolio/blob/main/images/Survivalcurve.jpg" width="400" />

Is there a competitive advantage in how businesses manage their key assets?
<br> Predicting failures impacts the bottom line. Consider the following:
<br>
- Personnel Safety - catastrophic equipment failure can be deadly in certain industries.
- Inventory Management - avoid unplanned downtime by having parts when you need them, but, avoid having too much to keep costs down.
- Reducing costs - replacing equipment too early is wasteful, but, too late can lead to overtime costs to fix in off hours, and variation in planned throughput.
<br> <b>In this analysis, I use simulated jet engine data from NASA to predict whether an engine will fail within 30 cycles.</b>
#### [Part 1: Tools: R, Technique: Logistic Regression, extreme Gradient Boosting, Survival Analysis](https://htmlpreview.github.io/?https://github.com/deloresmincarelli/Portfolio/blob/main/RUL_NASA_Engines.html)
#### [Part 2: Tools: Python, Technique: Long Short Term Memory Neural Network LSTM](https://htmlpreview.github.io/?https://github.com/deloresmincarelli/JetEngineLSTM/blob/main/JetEngineLSTM.html)
<br> 

## Project :  Predict Diabetes, Save results to database,  and use Natural Language to query the results
This project not only used auto-machine-learning for classification, it included OpenAI to enable the user/customer to interact with the data.
<br> This image shows a question entered by the user, which was interpreted by OpenAI and converted to SQL.  The SQL was run against a database with the prediction results. 
<br> You can see the results displayed, along with the query.  Note, OpenAI had to join two tables with no guidance in order to answer this question.
><img src="https://github.com/deloresmincarelli/Portfolio/blob/main/images/diabetes_streamlit.jpg" width="1000" />
<br> Steps:
<br> 1. Use Auto Machine Learning to classify patients with diabetes (0/1). AutoML runs several models at once, tunes all of the hyperparameters, and provides results for each model for comparison.

#### [See results of AutoML](https://htmlpreview.github.io/?https://github.com/deloresmincarelli/Portfolio/blob/main/diabetes_model.html)

2. Create a sqlite database (using DBeaver software) and import the diabetes predictions generated in Step 1.
3. Use the OpenAI generative language model (LLM) to write natural language questions to query the data in the database.  (SUBSCRIPTION REQUIRED)
4. Provide a web interface for the user to enter their questions, and view the answer.

#### [See Web app and OpenAI code](https://github.com/deloresmincarelli/Portfolio/blob/main/diabetes_streamlit_app.py)
   
Tools: Python (H2O Auto ML , langchain Open AI,  streamlit ), OpenAI generative language model,  DBeaver for db creation

## Project : [Crime in Louisville: Analysis & Clustering](https://htmlpreview.github.io/?https://github.com/deloresmincarelli/Portfolio/blob/main/crimeLouisville.html)
I moved to Louisville in 2022 and decided to put my datascience skills to use by exploring public data on crime in my new home town. 
<b> Further,  I did not find any public advanced analytics on Louisville crime.  This is a new study! </b>
<br>
<br>
Questions Answered:
- What types of crimes occur? Where? When?
- Does the Kentucky Derby cause a spike in crime?
- Which zipcodes have similar crime patterns?
<br> Tools: R
<br> Technique: Kmeans clustering

<img src="https://github.com/deloresmincarelli/Portfolio/blob/main/images/CrimeCluster.jpg" width="500" />



## Project : [Nurse Scheduling Optimization](https://github.com/deloresmincarelli/Portfolio/blob/main/Optimization_Portfolio.pdf)
MS Business Analytics, University of Cincinnati
<br> <b> How do you juggle employee shift preferences with business needs, in a way that builds confidence in a fair system? </b>
In this paper, I explore an optimization model that could be used to automate this complex decision making, reducing the amount of time it takes a nurse manager to balance nurse self-scheduling requests with hospital requirements. This case study uses a specific department at a hospital in Cincinnati for initial data and business rules. This department was one of several chosen to prototype self-scheduling.

This case study uses data from one scheduling period, followed by 3 additional examples designed to force the model to make the best choice given the constraints and objective.

Tools:  Python vs 3.6 and the PuLP package.

<img src="https://github.com/deloresmincarelli/Portfolio/blob/main/images/NurseOpt.jpg" width="500" />

## Project : [Decision Making Under Uncertainty](https://github.com/deloresmincarelli/Portfolio/blob/main/DecisionUncertainty_Portfolio.pdf)

<br> MS Business Analytics, University of Cincinnati
<br> We have all had to make decisions when the information we have is uncertain or incomplete.  Decision-analysis techniques and simulation can help quantify what-ifs, worst-case, and best-case scenarios. 
<br> Use Case:  Motivated by an active hurricane season in 2020, I explore a framework to aide in a hospital evacuation decision.  This model includes random variables, a decision tree to quantify the cost of the decision, and simulation to explore the cost distribution.  
<br> Tools:  R, Palisade suite of software for decision tree, simulation

<img src="https://github.com/deloresmincarelli/Portfolio/blob/main/images/HurricaneDecision.jpg" width="500" />

[pptx file with notes: select "view raw"](https://github.com/deloresmincarelli/Portfolio/blob/main/DecisionUncertainty_Portfolio.pptx)




