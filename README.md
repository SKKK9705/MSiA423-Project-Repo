# Project Repository

<!-- toc -->

- [Project Charter](#project-charter)
- [Project Backlog](#project-backlog)

<!-- tocstop -->

## Project Charter 

### Vision

The product is a web APP which provides a transparent and accurate tool for virtual soccer teams founders in any soccer video game to predict overall scores of players in their teams, as well as to find players right for their teams.

### Mission

**Accuracy**

The product enables users to predict overall scores for players in their teams based on combinations on different input attributes, which includes: age, weight, strength, stamina, shot power, etc.

According to the predicted score, the product produces recommendations of players different positions to users.

**Transparency**

Users are available to monitor the process of prediction and recommendation when using the product. All scores, positions of players will be displayed.

### Success criteria 

**ML Metric**: 

- Predict player scores with Mean Squared Error of  lower than 10. 

**Business Metric**: 

- 80% of users select recommended players as members of their teams.

- $100,000 of yearly revenue generated by payed service and advertisements.

- 3000 active users after first year run of the product

- 0.8 Click Through Rate for users who open the APP

## Project Backlog

### Project Themes



### Project Epics

**Main Page**

**Prediction**

**Recommendation**

### Project Timeline

**Week 1-2: Data Processing**

- Exploratory Data Analysis

  * Data Overview

    The dataset contains information on 18,207 players. Each player has unique ID and name with 85 attributes.

    + Descriptive Statistics
    + Skewness
    + Influential Observations

  * Data Cleaning
      
      + NAs Removing
      + Duplicates Removing
      + Outliers Removing
      + Invalid Attributes Removing

- Model Building

  Train multiple models to predict scores of players, including both linear and non-linear models. 
  
  * Linear Regression
  * Neural Network
  * Random Forest
  * Decision Tree
  
  MSE is the common measurement of performances for all models listed above. The model with the lowest MSE will be selected as the final model deployed in the product.

**Week 3-8: APP Building**

Build pipelines and web APP

**Week 9-10**

- Test web APP 

- Optimize user interfaces and write the final report.


<!--stackedit_data:
eyJoaXN0b3J5IjpbNzQ5NTIxNTE5LC04NTc3MzAyMDMsODU5NT
IxNzgxLC0xMTUyMzI0NDIxLDExNjg5ODYxOCwtMTI3NTA1ODU4
OCwtMTQzMzEwNjgzOCwtMTQ5OTYzNzE0NiwtMjI5MDg5MTUxLD
E3ODg3OTQwMTYsMTUxOTc2NzA0NCwtOTgyNTUxNjI0LC04ODUx
OTQzNiw1NTQ0NzQ4MzcsMTU3MDEzNTkxMiwxNzU4MTIzMzk3LD
MyODA5MDgyNSw1OTM3MTg4NDIsLTExNDA4MDkxOTcsNzk5MzM4
NTQwXX0=
-->