# deep-learning-challenge
Applying the Machine Learning and Neural Network:
1.	Overview: The purpose of this project is to assist the nonprofit foundation Alphabet Soup to select the applicants for funding with the best chance of success in their ventures.
2.	Results:
a.	Data Processing
i.	What variable(s) are the target(s) for your model? – The target variable is the ‘IS_SUCCESSFUL’ column from the DataFrame application_df
<img width="756" alt="image" src="https://github.com/tnguy25/deep-learning-challenge/assets/125770693/8f856ef7-e856-48eb-a305-8df5349fc82c">

ii.	What variable(s) are the features for your model? -  The feature variables are:
•	APPLICATION_TYPE-Alphabel Soup application type
•	AFFILIATION-Affiliated sector of industry
•	CLASSIFICATION-Government organization classification
•	USE_CASE-Use case for funding
•	ORGANIZATION-Organization type 
•	STATUS-Active status 
•	INCOME_AMT-Income classification
•	SPECIAL_CONSIDERATIONS-Special consideration for application
•	ASK_AMT-Funding amount requested
iii.	What variable(s) should be removed from the input data because they are neither targets nor features? – Both ‘EIN’ and ‘NAME’ was dropped from the input data.
<img width="736" alt="image" src="https://github.com/tnguy25/deep-learning-challenge/assets/125770693/4f901a80-1a0a-4931-9609-eaf8fab594fc">


b.	Compiling, Training, and Evaluating the Model
i.	How many neurons, layers, and activation functions did you select for your neural network model, and why? – There are 2 hidden layers. Layer 1 has 80 neurons and layer 2 has 30 neurons. Activation functions for hidden layers is ‘relu’ and for output later is ‘sigmoid’. Reason to choose the model: I was just guessing the neurons.
ii.	Were you able to achieve the target model performance? – I was unable to achieve 75% accuracy.
iii.	What steps did you take in your attempts to increase model performance? – I removed extra features ‘STATUS’, ‘SPECIAL_CONSIDERATIONS’, and ‘ASK_AMT’. For attempt number 1, I ran the code again and get the accuracy of 72.43%. Then, for attempt number 2, I changed the activation function of the hidden layers to “tanh” and output function to “relu”. For the last attempt, I add additional layer with 30 neurons. Activation functions for all hidden layer is “tanh” and output layer is “relu”.
4.	Summary: Overall, the deep learning model is approximately 73%. Additional layers with more neurons can be added to improve the result. Moreover, we can use the sequential model with keras-tuner library with hyperparameter option. In this case, we can allow kerastuner to decide activation functions and number of neurons to use in the hidden layers.
