# Deployment of a Rule based Healthcare chatbot as a Flask App

## Parts of the project:

### Classification model:
To classify various diseases based on their symptoms, Descision tree classifier is used. Descision tree algorithm here uses a recurse function that recursively traverses the tree to identify the disease based on symptoms entered by the user. It asks the user questions about symptoms until it reaches a lead node that corresponds to a disease. It then calls sec_predict() function which contains the in built descision tree classifier trained on our data, which also predicts the disease based on user symptoms. The two predicted diseases are compared. If they are same, the user has that disease. Otherwise, the user has possibility of one of the predicted diseases. After disease prediction, the description and precautions related to the disease are displayed.

### Step by step explanation:
1. First of all,chatbot asks the username.Then, it asks the disease symptom the user's facing.
2. Based on the user input, chatbot prompts the related diseases to choose from.
3. After the user chooses the disease symptom , the chatbot retrieves a list of symptoms based on the first symptom and asks the user one by one that if he has that particular symptom.
4. After obtaining the list of all symptoms experienced by user, the chatbot predicts the disease.
5. Various session variables are used to store user response and other variables to use later in the application.
                     
            
