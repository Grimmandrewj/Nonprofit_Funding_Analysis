## Analysis Overview - Purpose of Analysis
- The purpose of this analysis was to assist the nonprofit foundation Alphabet Soup to create a tool to help it select the applicants for funding with the best chance of success in their ventures
- In order to do so, I was to utilize my knowledge of machine learning and neural networks, using the features in the charity dataset (representing over 34,000 organizations) to create a binary classifier
- Using this classifier, I was to predict whether applicants will be successful if funded by Alphabet Soup

## Method and Results
Data Preprocessing
  - The variable from the dataset that was the target for the model was the column "IS_SUCCESSFUL," which showed 1 if funding was used effectively and 0 if not
  - The variables from the dataset making up the features were the remaining columns including "APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS," and "ASK_AMT."
  - The variables that were removed from the dataset as they represented neither targets nor features were the columns "EIN" and "NAME"

Compiling, Training, and Evaluating the Model
  - Initially, I selected 2 layers using the ReLU activation function and later altered the size of each layer and for    the third attempt added a third hidden layer.  This was to determine if altering the size and number of layers        would result in further optimization.  In my 2nd and 3rd attempts, I also altered the amount of columns removed        from the dataset for further optimization
  - Unfortunately, even with these alterations, I was unable to achieve 75% accuracy after 100 epochs using each of      the 3 models.  The results of each model are as follows: 
 
Model 1

![image](https://github.com/Grimmandrewj/Deep-learning_Challenge/assets/120341249/b781c65f-12c7-4451-871a-4e6620c78de7)

![image](https://github.com/Grimmandrewj/Deep-learning_Challenge/assets/120341249/8e84d53a-3191-468b-95bb-4430052395af)

Model 2

![image](https://github.com/Grimmandrewj/Deep-learning_Challenge/assets/120341249/8821f87b-8b03-4cc6-b955-d9ac71e1e7f1)

![image](https://github.com/Grimmandrewj/Deep-learning_Challenge/assets/120341249/2d8516af-618d-4e40-a2d0-639eea1da5b6)

Model 3

![image](https://github.com/Grimmandrewj/Deep-learning_Challenge/assets/120341249/a75fce53-b7ac-4e1e-a3d3-23a27d1e4059)

![image](https://github.com/Grimmandrewj/Deep-learning_Challenge/assets/120341249/78d3a1da-2a81-4273-b63c-8dfebb46f07d)

## Summary
- Though alterations were made to attempt to optimize the accuracy of each model, the overall accuracy did not vary greatly between them (72.5%, 72.6%, 72.9%).  Altering the amount and size of the layers and amount of neurons did not yield the desired result of 75% accuracy and in fact did not significantly change the overall accuracy nearly at all
- I believe with further evaluation of the dataset, modification of the parameters, and alteration of the models may result in greater accuracy results if I was able to continue to familiarize myself with this process.   
