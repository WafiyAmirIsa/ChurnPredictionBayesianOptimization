# Model Card

## Model Description

**Input:** The inputs to the models are the various attributes in the Cell2Cell dataset used to identify customer churn in a telecommunication company.

**Output:** The output of the models is a binary classification of whether a customer is likely to churn or not.

**Model Architecture:** The models used include Naive Bayes, Decision Tree, Logistic Regression, Support Vector Machine, Adaboost, Multi-Layer Perceptron Classifier, and Voting Classifier. Each model was trained on a separate subset of the dataset, and the best-performing models were selected using Bayesian optimization.

## Performance

I evaluated the models on accuracy, F1 score, precision, and recall using a 60/40 train-test split of the dataset. The best-performing model is Support Vector Machine which had an accuracy of 73.8%, an F1 score of 63.0%, a precision of 70.2%, and a recall of 73.8%.

## Limitations

One of the limitations of the model is that it was trained using an unbalanced class of various attributes, which may be sensitive to bias. This can also limit the use of certain machine learning algorithms. Additionally, some of the models, such as the decision tree, may exhibit bias due to the unbalanced class distribution in the dataset.

## Trade-offs

To address the trade-off of using machine learning models that may be sensitive to bias, we have employed different machine learning models that are less likely to exhibit bias. By using a diverse range of models and techniques, we can improve the robustness and generalizability of the model, thereby reducing the impact of potential biases and performance issues.
