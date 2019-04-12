# Prediction and Recommendation on Players for Virtual Soccer Team

<!-- toc -->

- [Project Charter](#project-charter)
- [Project Planning](#project-planning)
- [Backlog](#backlog)
- [Icebox](#icebox)


<!-- tocstop -->

## Project Charter 

### Vision

The product is a web APP which provides a transparent and accurate tool for virtual soccer teams founders in any soccer video game to predict overall scores of players in their teams, as well as to find players right for their teams.

### Mission

Accuracy and transparency are product goals.

**Accuracy**

The product enables users to predict overall scores for players in their teams based on combinations on different input attributes, which includes: age, weight, strength, stamina, shot power, etc.

According to the predicted score, the product produces recommendations of players different positions to users.

**Transparency**

Users are available to monitor the process of prediction and recommendation when using the product. All scores, positions of players will be displayed.

### Success criteria 

**ML Metric**: 

- Less than 10 of Mean Squared Error to predict  scores of players

- More than 0.7 of R-Squared for the final model

**Business Metric**: 

- 80% of users select recommended players as members of their teams.

- $100,000 of yearly revenue generated by payed service and advertisements.

- 3000 active users after first year run of the product

- 0.8 Click Through Rate for users who open the product

## Project Planning

### Theme

The theme of this product is to help users easily predict overall player scores and choose the best player for their virtual soccer teams.

### Epics

- Epic 1: Exploratory Data Analysis

    The dataset contains information on 18,207 players. Each player has unique ID and name with 85 attributes. The response variable is overall score and the rest of the attributes are possible independent variables. Overall description of the data includes following categories.

  * Story 1: Data Overview

    + Descriptive Statistics
    
        Construct a summary on the data, including total count of observations, minimum value, maximum value, mean and median for each attribute.
        
    +  Skewness
    
        Draw histograms for all attributes with numerical values to see the skewness. For models that require normal distribution, log transform attributes that are left or right skewed.
      
    + Influential Observations
    
        Check all observations with extreme values, for example, observations with some attributes of lower than 0 or larger than 100.

  * Story 2: Data Cleaning
      
      + NAs Removing
       
         Remove observations having NA values for selected variables. 
         
      + Duplicates Removing
        
        Remove duplicated observations, which are defined as observations sharing the same unique player ID.
        
      + Outliers Removing
      
        Remove all abnormal observations that could have impact on parameters of the model.
      
      + Invalid Attributes Removing
     
        Remove attributes that will not be selected to build models, such as player ID, player photo, player nationality, player club and club logo.

- Epic 2: Model Building

  Using the given dataset, find the best model to predict player scores and recommend players.
  
  * Story 1: Model Fitting

    Randomly split the dataset into training set and test set with proportions of 80% and 20% respectively. Use training set to fit multiple models to predict scores of players, including both linear and non-linear models. 

    +  Linear Regression
    + Neural Network
    + Random Forest
    + Support Vector Machine
  
  * Story 2: Model Comparison  
  
    MSE is the common measurement of performances for all models listed above. After running a 10-fold cross validation for 10-times, the model with the lowest mean MSE will be selected as the final model deployed in the product.

- Epic 3: Product Building

  * Story 1: Web APP Building  
   
    + Build pipelines
    + Realize all functions of the web APP
  
  * Story 2: Web APP Connection
   
    + Link different parts of the web APP together

- Epic 4: Product Refinement

  * Story 1: Product Test  
    
    Use sample data to test the feasibility of the product, including:
    
      + Accuracy of prediction model
      + Accuracy of recommendation system
      + Work flow of the product
      + Work speed of the product

  * Story 2: Product Refinement
  
    Find drawbacks of the product and propose possible refinements correspondingly.

  * Story 3: Product Summary
  
    Write instructions of the product and the final report of the project.

## Backlog

1. "Theme.Epic1.Story1" Data Overview (2 points) - Planned
2. "Theme.Epic1.Story2" (2 points) - Planned
3. "Theme.Epic2.Story1" (4 points)
4. "Theme.Epic2.Story2" (4 points)
5. "Theme.Epic3.Story1" (8 points)
6. "Theme.Epic3.Story2" (8 points)
7. "Theme.Epic4.Story1" (4 points)
8. "Theme.Epic4.Story2" (4 points)
9. "Theme.Epic4.Story3" (8 points)

## Icebox

"Theme.Epic2.Story1"
"Theme.Epic3.Story1"

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTQ1ODkwNTMwMCwtMjk5MTkwNTY2LC01MT
M2MjczNTMsMjc3MTEwNzcxLDYwNDY1NzA3NiwtODQzNTMxMTk1
LDYxNzU3Mjg2MCwyMDMzMzc2NTU1LC0yNTk5MTMyMDcsLTgyMz
EzMDM5NSwtOTM3OTQ0MCw4MDM5ODQ2ODMsMTc3NTgwNjM1MCw4
NDkzMTc4OTQsMTI1MjYzNjY1NywxOTg2NDg3Mjk4LC0xNzA4OD
I3NDA5LDEwMzQzMTYzMDcsNTEwMTc0NDI1LC0yMTA1OTM5Njg4
XX0=
-->