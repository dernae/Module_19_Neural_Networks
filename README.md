## Overview of The Analysis 

The purpose of this analysis is to create a binary classifier that is capable of predicting whether 
applicants will be successful if funded by a certain company. The analysis utilized a CSV containing
more than 34,000 organizations that have received funding from the business over the years using the 
Deep Learning Macchine Learning Model. 

## Results

   ### Data Preprocessing 
   
   - The target variable for this model is the columns:"IS_SUCCESSFUL"-- whether the efficiency of the 
      money use was successful or not. 
   - The variables considered to be features after optimization were the columns: application type, 
     'AFFILIATION' -- affiliated, 'CLASSIFICATION'--sector of industry, 'USE_CASE'--use case for 
      funding and 'INCOME_AMT'--Funding amount requested
   - The variables that were neither targets nor features include: Identification columns
      ("EIN", "NAMES"),"SPECIAL_CONSIDERATIONS"--Special consideration for application,
       "ORGANIZATION"--Organization type.

   ### Compiling, Training, and Evaluating the Model
   - Overall, I used three neurons and three hidden layers as well as the "sigmoid" function for all 
     activation functions for the input data and the "tanh" function. 
   - Unfortunately, I was not able to achieve the target level performance of 75%. After attempted 
      optimization, the model achieves 53% accuracy. 
   - To optimize the model, I tried dropping additonal columns including "SPECIAL_CONSIDERATIONS"
     and "ORGANIZATION"; Adding more neurons and hidden layers and using different activation 
     functions for both output and input data.
 
## Summary
Using the Deep Learning Macchine Learning Model, I attempted a myriad of techniques to increase the 
accuracy to the target 75%. Initially, I used the "relu and "sigmoid" functions for the input and
output respectively. For optimization, the variables that were neither targets nor features include: 
Identification columns("EIN", "NAMES"),"SPECIAL_CONSIDERATIONS"--Special consideration for application,
"ORGANIZATION"--Organization type. The optimization proved unsuccessful as the accuracy decreased from 
60.3% to 53.2%. For a dataset that is similar to 5 rows and 38 of initial columns, I recommend utilizing
the Random Forest Machine Learning Model for its efficiency, readability and accuracy.
