# Bike Sharing Case Study
---
## Case study assignment by IIIT Bangalore and Upgrad
---
> - Solving this assignment will give an idea of analysing the dataset and build a model to predict the variable of interest. Here, the interest is to predict the demand for bike users based on few other parameters.
> - Developed as part of the Linear Regression Module required for Executive Post Graduate Program in Machine Learning and AI - IIIT,Bangalore.
---

## Table of Contents
* [General Information](#general-information)
* [Methodology](#methodology)
* [Repository contents](#repository-contents)
* [Conclusions](#conclusions)

## General Information
A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

**The company wants to know:**
- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands.
  
**Objective:**
Build a **model** for the demand of shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features.

## Methodology
1) Reading and Understanding the Data
2) Data manipulation and cleaning
3) Visualising the Data
4) Data Preparation
5) Splitting the Data into Training and Testing Sets
6) Building model
7) Residual Analysis of the train data
8) Making Predictions Using the Final Model
9) Model Evaluation

## Repository contents
| File | Description |
|:-----|:------------|
| Python notebook | It contains the complete detailed code along with necessary output to solve the problem|
| PDF | Answered the asked subjective questions. |
| README.md | This file briefs about the project. |
| day.csv | The bike sharing case study data set. |
| data_dictionary.txt | Meaning of the variables in the dataset. |

## Conclusions
By using **RFE approach and manual selection** for finding the predictors, we have derived the following conclusions.

**Intercept :**  0.27214083391522237

_Below are the predictors used in the final model based on their ranking:_
| Ranking | Predictor |	Coefficient |
|:--------|:----------|:------------|
|1|	temp |	0.351334 |
|2|	weathersit_bad |	-0.342787 |
|3|	yr |	0.230702 |
|4|	season_spring |	-0.166929 |
|5|	holiday |	-0.088471 |
|6|	mnth_sept |	0.094459 |
|7|	weathersit_moderate |	-0.078991 |
|8|	mnth_oct |	0.076377 |

_Based on these values, below is the multiple linear model equation:_

$cnt = 0.272141 + \\left( 0.351334 \\times temp \\right) - \\left( 0.342787 \\times weathersit\\_bad \\right) + \\left( 0.230702 \\times yr \\right) - \\left( 0.166929 \\times season\\_spring \\right) - \\left( 0.088471 \\times holiday \\right) + \\left( 0.094459 \\times mnth\\_sept \\right) - \\left( 0.078991 \\times weathersit\\_moderate \\right) + \\left( 0.076377 \\times mnth\\_oct \\right)$

_From the above ranking table, we can derive the following predictors as signifcant in order:_
1) Temperature
2) Weather
3) Year
4) Season
5) Holiday
6) Month

_Below are few inferences from the analysis, the demand for bikes:_
- Increase when temperature increase => The company can expect high demand during high temperature.
- Increase every year => The company should focus on staying in business.
- Increase around September and October month => The company should prepare to manage the demands.
- Decrease during holidays => The company can promote offers, campaigns, tournament or etc. to make people use during the holidays.
- Decrease during spring and when weather is not good => It might be because of difficulty for the user during these bad conditions which is not good for driving. Hence, company can focus on preparing for meeting higher demands later like servicing the bikes, repairing the bike docks etc.

## Contact
Created by [@shruthipv96] - feel free to contact me!
