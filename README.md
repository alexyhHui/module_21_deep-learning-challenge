# module_21_deep-learning-challenge

## Overview 

The purpose of this analysis was to develop a deep learning model using TensorFlow and Keras to predict whether organizations funded by Alphabet Soup would be successful based on various features provided in the dataset. The dataset contained information about these organizations, including their application type, classification, and other relevant features.

## Results

### Data Preprocessing
- What variable(s) are the target(s) for your model?

  The target variable for our model was `IS_SUCCESSFUL`, indicating whether the organization was successful or not.

- What variable(s) are the features for your model?

  The features for our model included various characteristics of the organizations such as `APPLICATION_TYPE`, `CLASSIFICATION`, `AFFILIATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS` and `ASK_AMT`.

- What variable(s) should be removed from the input data because they are neither targets nor features?

  The `EIN` and `NAME` columns are removed from the input data as they were neither targets nor features.

### Compiling, Training, and Evaluating the Model

Original attempt
- Model: Sequential model with two hidden layers (80 neurons and 30 neurons) and ReLU activation.
- Result: Achieved an accuracy of 72.73% and loss of 55.69%.

1st Attempt
- Model: Sequential model with two hidden layers (200 neurons and 80 neurons) and ReLU activation.
- Result: Achieved an accuracy of 72.63% and loss of 56.38%.

2nd Attempt
- Model: Sequential model with three hidden layers (80 neurons, 30 neurons, and 5 neurons) and ReLU activation.
- Result: Achieved an accuracy of 72.38% and loss of 55.61%.

3rd Attempt
- Model: Sequential model with three hidden layers (200 neurons, 80 neurons, and 10 neurons) and ReLU and Tanh activation.
- Result: Achieved an accuracy of 72.59% and loss of 55.68%.

## Summary

- Despite various attempts at optimizing the model by adjusting the architecture and hyperparameters, the accuracy remained around 72-73%.
- It seems that adding more neurons or layers did not significantly improve the model's performance.
- Further experimentation with different activation functions, regularization techniques, or optimization algorithms could be explored to enhance the model's accuracy.

It's also essential to consider the possibility of data imbalance or noise in the dataset, which may affect the model's performance.
Overall, while the model achieved reasonable accuracy, further refinement may be necessary to achieve the desired target accuracy of over 75%.
