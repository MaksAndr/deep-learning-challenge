# deep-learning-challenge
Report

Overview of the Analysis:


The objective of this analysis is to develop a new predictive tool using a neural network or deep learning model to estimate the likelihood of success for applicants receiving funding from Alphabet Soup. The model will be trained on a comprehensive dataset that includes relevant features and success labels, which will be preprocessed and cleaned to ensure data quality. The chosen neural network architecture will be trained using an appropriate optimization algorithm and loss function, while monitoring its performance on a separate validation dataset to prevent overfitting. The goal is to optimize the model's parameters to minimize prediction errors and achieve an accuracy rate exceeding 75%, ensuring the reliability and accuracy of the model in predicting the success of Alphabet Soup-funded organizations.



Results:

Data Preprocessing
1.What variable(s) are the target(s) for your model?
The target variable(s) for the model is IS_SUCCESSFUL

2.What variable(s) are the feature(s) for your model?
All the other columns except IS_SUCCESSFUL.

3.What variable(s) should be removed from the input data because they are neither targets nor features?
During the analysis, the variable "EIN" was initially dropped from the input data as it was determined to be irrelevant for predicting the success of Alphabet Soup-funded organizations. This variable did not contain any meaningful information and was not useful for the analysis. However, the "NAME" column, which provides the names of the organizations, was considered to have potential relevance and was included as a feature in the model. The "NAME" column could potentially contain informative details that could contribute to predicting the success of applicants.



Compiling, Training, and Evaluating the Model:


1.How many neurons, layers, and activation functions did you select for your neural network model, and why?


In the initial model, three hidden layers were utilized, consisting of 100, 40, and 1 neurons, as specified in the provided starter code. The activation functions chosen were "relu" for the hidden layers and "sigmoid" for the output layer. The input dimension of the model was determined by the length of the input features, ensuring compatibility with the dataset used for training.

![first](https://github.com/MaksAndr/deep-learning-challenge/assets/119984723/96d38f85-269c-4e6b-b76f-5f61eb6faa61)


2.Were you able to achieve the target model performance?

The initial model did not meet the desired target performance. 

![second](https://github.com/MaksAndr/deep-learning-challenge/assets/119984723/949d9d29-87ad-40ea-bcde-04249a693fe5)

3.What steps did you take in your attempts to increase model performance?

After several attempts to improve the model's performance, the second and third iterations proved to be successful in achieving the desired target model performance. The accuracy of the models in these later attempts surpassed the threshold set for the analysis, indicating that the necessary optimizations and adjustments were made to enhance their predictive capabilities.
![third](https://github.com/MaksAndr/deep-learning-challenge/assets/119984723/7a0edac1-d6ac-4c67-8c7b-f1649f4aa542)

![forth](https://github.com/MaksAndr/deep-learning-challenge/assets/119984723/f4ebd91e-75f4-4be2-a8bc-9f35554318d9)  
   
  
The crucial step that significantly improved the model's performance was retaining the "NAME" column as a feature. By including this variable in the model, a notable enhancement in accuracy was observed. Additionally, introducing an additional hidden layer with a linear activation function slightly improved the model's overall performance. Ultimately, the decision to not drop the "NAME" variable played a vital role in optimizing the model, leading to the desired outcomes in AlphabetSoupCharity_Optimization2
![fifth](https://github.com/MaksAndr/deep-learning-challenge/assets/119984723/a450cc69-bc24-414c-b084-16ae8a7d05ba)

![sixth](https://github.com/MaksAndr/deep-learning-challenge/assets/119984723/ea9569ec-a562-4f98-b58e-659a421154a5)

  Summary:
   The model was optimized to achieve a 75% accuracy in predicting the success of organizations funded by Alphabet Soup. This means it could accurately determine whether an organization would be successful or not based on the given features. Although the model met the accuracy goal, there is still room for improvement in reducing prediction errors. To further enhance the model, a Random Forest classifier could be considered as an alternative. This classifier can handle different types of features, reduce overfitting, and provide insights into important features. Utilizing a Random Forest model may lead to better accuracy and performance in predicting the success of Alphabet Soup-funded organizations.

