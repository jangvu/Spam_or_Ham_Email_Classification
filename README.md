# Spam_or_Ham_Email_Classification
Spam emails are unwanted emails share in bulk intending to gather data/ do phishing/ perform social engineering/ start an attack and a lot more – mostly for bad causes.
In this small project, I will try to classify the spam or ham email by using the data from Kaggle.

The Pipeline of this project 
![Spam_or_ham drawio](https://github.com/jangvu/Spam_or_Ham_Email_Classification/assets/50269219/48ed9582-6de5-4ba4-b211-57d2531b2ae7)


1. Preprocessing Data

There is a imbalanced in the training data, in order to solve this problem. A downsampling function is used to balance the amount of training data between spam and ham label

<img src="https://github.com/jangvu/Spam_or_Ham_Email_Classification/assets/50269219/f8dc3b4d-dcfd-4b68-bb85-01cb4208fb90" alt="Imbalanced Data" width="100" height="100">



One-hot Encoding is used to reduce the computational cost, in which
* 1 – If a category is a ham/ not spam
* 0 – if the category is spam

2. Transfer-learning BERT

There are 2 main components: bert_preprocessor and bert_encoder, and both of them are pretrained.

As a generic step in the model building, we will now compile our model using adam as our optimizer and binary_crossentropy as our loss function. /For metrics, we will use accuracy, precession, recall, and loss.

3. Evaluation and Prediction

![image](https://github.com/jangvu/Spam_or_Ham_Email_Classification/assets/50269219/6ce03fbe-351e-452f-868b-595b084abbaf)
