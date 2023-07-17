# Deep-Learning-Challenge

**Overview of Analysis:** 
The purpose of this analysis is to build a machine learning model to help a company select funding applciants that are most likely to be successful in their endeavors.

**Results:**

*Variable Descriptions*
* What variable(s) are the target(s) for your model? The 'Is_Successful' column is the target (what we're looking to predict)
* What variable(s) are the features for your model? The features of this model are: 'Application_Type', 'Affiliation', 'Classification', 'Use_Case', 'Organization', 'Status', 'Income_Amount', 'Special_Considerations', and 'Ask_Amt' (what will help us predict the outcome)
* What variable(s) should be removed from the input data because they are neither targets nor features? We removed the 'Ein' and 'Name' variables

*Compiling, Training, and Evaluating the Model*
* How many neurons, layers, and activation functions did you select for your neural network model, and why? 12 neurons (as increasing neurons throughout the trials lead to slight improvements in accuracy), 3 layers (as adding an additional layer also helped slightly improve accuracy) and the Relu activation function (as it is most commonly used in deep learning).
* Were you able to achieve the target model performance? After turning the model (by adding additional neurons, changing the activation function, and adding an additional layer) I was not able to achieve the target model performance (where accuracy >= 75%)
  
(<img width="620" alt="image" src="https://github.com/kristenfarabaugh/Deep-Learning-Challenge/assets/123901701/7afc7549-348b-4fa7-9bdb-5cdf075cf1e5">)
* What steps did you take in your attempts to increase model performance? I added additional neurons, changed the activation function and added an additional layer in three attempts to increase model performance vs the original pass.

**Summary of Results:**
After three attempts at hyperparameter tuning, the model was only able to perform at a 73% accuracy (below the target of 75%). This means the model can only correclty predict the success of a funding applicant 73% of the time, and should not be implemented (as it does not meet the baseline target and creates risk for the company). We can attempt to improve the accuracy by looking into a few different things: 1) using Kerastuner - does the set of ideal parameters increase accuracy above the desired threshold? 2) looking into the features - are some of the model inputs confusing, inadquate or outliars? 
