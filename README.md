# Deployment of a Rule based Healthcare chatbot as a Flask App

## Parts of the project:

### Classification model:
To classify various diseases based on their symptoms, Descision tree classifier is used. Descision tree algorithm here uses a recurse function that recursively traverses the tree to identify the disease based on symptoms entered by the user. It asks the user questions about symptoms until it reaches a lead node that corresponds to a disease. It then calls sec_predict() function which contains the in built descision tree classifier trained on our data, which also predicts the disease based on user symptoms. The two predicted diseases are compared. If they are equal, the user has that disease. Otherwise, the user has possibility of one of the predicted diseases. After disease prediction, the description and precautions related to the disease are displayed.
                     
            
