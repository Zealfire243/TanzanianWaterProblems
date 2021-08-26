# TanzanianWaterProblems
## Overview

A one-paragraph overview of the project, including the business problem, data, methods, results and recommendations.

## Business Problem

Tanzania has issues providing clean water to its population of over 57,000,000. Through a competition on DrivenData.org I have been tasked to analyze and predict which water pumps will need to be repaired in the future. Understanding what water pumps will need repairs can improve maintenace costs and time, and ensure the availability of clean water to Tanzanians.

## Data

Describe the data being used for this project.
The data I am using was sourced from Taarfia and The Tanzanian Ministry of Water. Given that this data is from a competition I know that it perfectly relates to the business problem. The data gives information about the location of the water point, what type of pump is being used, how its being managed and when it was installed. Using this information I need to predict whether a pump is functional, needs some repairs or doesn't work at all.


## Methods

First to analyze I dove into looking through all the value counts for my variables. Looking to figure out which columns I was going to use. What I was looking for was medium variety, high null value count, checking for null replacement values etc. This was a ternary classification problem however I converted it to a binary classification problem to save on time. After cleaning I decided to go with a simple GridSearchCV Decision Tree Classifier. I did a simple model instead of a more complicated one because I want to know which variables are affecting my model the most. My first step was hyperparameter tuning of which the results for accuracy can be found below.
![MaxDepths](./Images/MaxDepths.png)
![MaxFeatures](./Images/MaxFeatures.png)
![MinSamplesLeafs](./Images/MinSamplesLeafs.png)
![MinSamplesSplits](./Images/MinSamplesSplits.png)
![MinWeightFractionLeafs](./Images/MinWeightFractionLeafs.png)
I used these results to find a starting point for my Grid Search to build my final model. 

## Results


![ConfusionMatrix](./Images/ConfusionMatrix.png)
***
Questions to consider:
* How do you interpret the results?
* How confident are you that your results would generalize beyond the data you have?
***

Here is an example of how to embed images from your sub-folder:




## Conclusions

Provide your conclusions about the work you've done, including any limitations or next steps.

***
Questions to consider:
* What would you recommend the business do as a result of this work?
* What are some reasons why your analysis might not fully solve the business problem?
* What else could you do in the future to improve this project?
***

## For More Information

Please review our full analysis in [our Jupyter Notebook](./dsc-phase1-project-template.ipynb) or our [presentation](./DS_Project_Presentation.pdf).

For any additional questions, please contact **name & email, name & email**

## Repository Structure

Describe the structure of your repository and its contents, for example:

```
├── README.md                           <- The top-level README for reviewers of this project
├── FinalProduct.ipynb   <- Narrative documentation of analysis in Jupyter notebook
├── TanzanianWaterPresentation.pdf         <- PDF version of project presentation
├── data                                <- Both sourced externally and generated from code
└── Images                              <- Both sourced externally and generated from code