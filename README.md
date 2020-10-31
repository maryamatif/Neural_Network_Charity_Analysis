# Neural_Network_Charity_Analysis

## Overview of the analysis:
The challenge was to analyze a huge list of data regarding 34000 organizations to determine whether each applicant was succesful if they received funding from Alphabet Soup. There was alot of data regarding amount funded, organization type, special considerations etc. We analyzed the data for a neural network model. 

## Results: Using bulleted lists and images to support your answers, address the following questions.

### Data Preprocessing
### What variable(s) are considered the target(s) for your model?
IS_SUCCESSFUL varialbe was considered the target of our model. It determines whether the money given was used succesfully or not. 

### What variable(s) are considered to be the features for your model?
The following variables were used as features or independent variables for the model: 
Application type
Affiliation
Classification
Use_case
Organization
Status
Income_amt
Special_considerations
Ask_amt

### What variable(s) are neither targets nor features, and should be removed from the input data?
Variables that don't provide any useful information in terms of predicting the results should be removed. Those would be the following:
EIN
Name

### Compiling, Training, and Evaluating the Model
### How many neurons, layers, and activation functions did you select for your neural network model, and why?
first hidden layer: Neurons: 80. Activation function: relu
second hidden layer: Neurons: 30. Activation function: relu
Output layer: Activation function: Sigmoid

### Were you able to achieve the target model performance?
No, the accruacy figure for the inital model was 72%. Our target was 75%.

### What steps did you take to try and increase model performance?
1. I tried removing the special considerations column as well. 
2. I decreased the bins for the classifcation variable. 
3. I increased the neurons for the model for each layer.
4. I added another layer to the model.

### Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.

The deep learning model for the alphabet soup was only able to predict 73% of the outcomes correctly at maximum. Depending on the company's objectives and accuracy standards, this model could be considered accurate enough or not. We could use a different model such as random forest classifier for solve this problem. I suggest that model due to it's speed and implementation complexity, both of which are superior to the neural network. Random forest is much faster and easier to establish than the neural model and hence could've saved the company time and resources, even if the prediciton results would be more or less the same. 
