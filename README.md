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

- 0.8 Click Through Rate for users who open the product

## Project Backlog

### Project Themes

**Prediction**

**Recommendation**

### Project Epics

**Main Page**

**Prediction Page**

**Recommendation Page**

The product will filter players in the dataset of scores within 1 point range of predicted outcomes.

### Project Timeline

**Week 1-2: Data Processing**

- Exploratory Data Analysis

  * Data Overview

    The dataset contains information on 18,207 players. Each player has unique ID and name with 85 attributes. The response variable is overall score and the rest of the attributes are possible independent variables.

    + Descriptive Statistics
    + Skewness
    
      Draw histograms for each attribute with numerical values. Some models require 
      
    + Influential Observations

  * Data Cleaning
      
      + NAs Removing
      + Duplicates Removing
      + Outliers Removing
      + Invalid Attributes Removing
     
        Remove attributes that will not be selected to build models, such as player ID, player photo, player nationality, player club and club logo.

- Model Building

  Train multiple models to predict scores of players, including both linear and non-linear models. 
  
  * Linear Regression
  * Neural Network
  * Random Forest
  * Decision Tree
  
  MSE is the common measurement of performances for all models listed above. The model with the lowest MSE will be selected as the final model deployed in the product.

**Week 3-8: Product Building**

- Build pipelines

- Realize all functions of the product 

- Link different parts of the product together

**Week 9-10**

- Test the product 

- Optimize user interfaces 

- write the final report.


<!--stackedit_data:
eyJoaXN0b3J5IjpbNzQ2Nzc0MjQ5LC0xODg5MDA5MzQzLC04NT
c3MzAyMDMsODU5NTIxNzgxLC0xMTUyMzI0NDIxLDExNjg5ODYx
OCwtMTI3NTA1ODU4OCwtMTQzMzEwNjgzOCwtMTQ5OTYzNzE0Ni
wtMjI5MDg5MTUxLDE3ODg3OTQwMTYsMTUxOTc2NzA0NCwtOTgy
NTUxNjI0LC04ODUxOTQzNiw1NTQ0NzQ4MzcsMTU3MDEzNTkxMi
wxNzU4MTIzMzk3LDMyODA5MDgyNSw1OTM3MTg4NDIsLTExNDA4
MDkxOTddfQ==
-->