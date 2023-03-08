# codeless-ai-ml-2022
# Introduction
Employee Attrition is when an employee leaves the company through any method, including voluntary resignations, layoffs, failure return from leave of absence, or even illness or death. Every year a lot of companies hire a number of emplyoyees. The companues invest time and money in trining those employees, not just this but there are training programs within the companies for thire existing employees as well.

# Research Idea
1.Use data to predict employee attrtion.
2.Use data to let companies know their weaknesses from an employee's point of view. in order to make adjustments and may reduce the number of employees who will resign Or it can make employees happier and improving the performance of employees.

# Overview of the Study
Our studying concerns the gender , satisfaction level of employee with work environment and company , frequency of business travel, department, salary bracket of employee and distance from home to office.
The specific objective of this Study was to investigate the advertising strategy employed by company to which group of people they must advertise more. Our goal was to compare purchasing of the product by person based on sex , age and estimated salary.
Our data focuses on internal reasons for employees leaving only. There may be external reasons or personal reasons for employees to resign, such as health, family conditions, death, etc.

# Tool
knime

# Nodes being used in KNIME
CSV Reader
Column Filter 
Partitioning
Decision Tree Learner
Decision Tree Predictor
Logistic Regression Learner
Logistic Regression Predictor
Naive Bayes Learner 
Naive Bayes Predictor
Random Forest Learner
Random Forest Predictor
Scorer 

# Model
*1. Data access and preparation/*
<p float="left">
 <img src="img/access and clean data.png" alt="image" width="50%"/> 
</p>
using CSV Reader node for access data.
In part of data preparation I use Column filter to remove columns that I don't need or are not important for use
and use Partitioning to divide information, The first is for the ML to learn and the other is for the ML to test, 
I divided into 90:10 , 80:20 , 70:30 to try to compare which one is the best.

*2.classification model (Decision Tree model)/*
<p float="left">
 <img src="img/decision tree.png" alt="image" width="50%"/> 
</p>
using Decision Tree Learner node and Decision Tree Predictor node.

*3.classification model (Naive Bayes model)/*
<p float="left">
 <img src="img/naive bayes.png" alt="image" width="50%"/> 
</p>
using Naive Bayes Learner node and Naive Bayes Predictor node.

*4.classification model (Random Forest model)/*
<p float="left">
 <img src="img/random forest.png" alt="image" width="50%"/> 
</p>
using Random Forest Learner node and Random Forest Predictor node.

*5.classification model (Logistic Regression model)/*
<p float="left">
 <img src="img/logistic.png" alt="image" width="50%"/> 
</p>
using Logistic Regression Learner node and Logistic Regression Predictor node.

*6.score of each classification model (Partitioning 90:10)/*
-Decision Tree model
<p float="left">
 <img src="img/decision-90.png" alt="image" width="50%"/> 
</p>
-Naive Bayes model
<p float="left">
 <img src="img/naive-90.png" alt="image" width="50%"/> 
</p>
-Random Forest model
<p float="left">
 <img src="img/random-90.png" alt="image" width="50%"/> 
</p>
-Logistic Regression model
<p float="left">
 <img src="img/logistic-90.png" alt="image" width="50%"/> 
</p>

*7.score of each classification model (Partitioning 80:20)/*
-Decision Tree model
<p float="left">
 <img src="img/decision-80.png" alt="image" width="50%"/> 
</p>
-Naive Bayes model
<p float="left">
 <img src="img/nive-80.png" alt="image" width="50%"/> 
</p>
-Random Forest model
<p float="left">
 <img src="img/random-80.png" alt="image" width="50%"/> 
</p>
-Logistic Regression model
<p float="left">
 <img src="img/logistic-80.png" alt="image" width="50%"/> 
</p>

*8.score of each classification model (Partitioning 70:30)/*
-Decision Tree model
<p float="left">
 <img src="img/decision-70.png" alt="image" width="50%"/> 
</p>
-Naive Bayes model
<p float="left">
 <img src="img/naive bayes-70.png" alt="image" width="50%"/> 
</p>
-Random Forest model
<p float="left">
 <img src="img/random forast-70.png" alt="image" width="50%"/> 
</p>
-Logistic Regression model
<p float="left">
 <img src="img/logistic-70.png" alt="image" width="50%"/> 
</p>

# Conclusion
In summary, using the naive bayes model and the logistic modal gives the best accuracy with a score of 85:15 in an 80:10 split, both of model fit this data best.
<p float="left">
 <img src="img/nive-80.png" alt="image" width="50%"/> 
</p>
<p float="left">
 <img src="img/logistic-80.png" alt="image" width="50%"/> 
</p>
