# charityData

Overview of the analysis: The purpose of this analysis is to determine whether or not applicants for charity grant funding will be successful. Alphabet Soup was used to create an algorithm to predict whether or not the applicant will be successful. A

Data Preprocessing

What variable(s) are the target(s) for your model? 
-The target for the model was the Is-Successful column.


What variable(s) are the features for your model?
-The features include: application_type, affiliation, classification, uce_case, organization, status, income, special_considerations, and ask amount


What variable(s) should be removed from the input data because they are neither targets nor features?
-EIN (Employee Identification), and NAME
-Ended up adding name back in when optimizing


Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
-For this model, 3 hidden layers were selected with many neurons because when there's several neurons the accuracy seems to increase. Initially, I tried relu, but switched to sigmoid when optimizing. The names were added back in and adjusted to increase accuracy. 



Were you able to achieve the target model performance?
After adding a third layer, and adding the name column back in, yes. 


What steps did you take in your attempts to increase model performance?
-Adding an additional layer didn't necessarily improve the performance completely. The Name column was re-added to the data and grouped to increase the size of the data being used in the model. This helped increase performance significantly and brought the accuracy up to 78%. 


Summary: The model had an overall accuracy of 78%. The applicant has a 78% chance of being successful if:

-The name of the applicant appears more than 5 times in the dataset
-The application type falls under T3, T4, T6, T5, T19, T8, T7, or T10. 
-The classification is C1000, C2000, C1200, C3000, C2100