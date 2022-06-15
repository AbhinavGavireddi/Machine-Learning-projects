# Sentiment Analysis

The goal of this project is to design a classifier to use for sentiment analysis of product reviews. Our training set consists of reviews written by Amazon customers for various food products. The reviews, originally given on a 5 point scale, have been adjusted to a +1 or -1 scale, representing a positive or negative review, respectively.
Each entry consists of the review and its label. 

In order to automatically analyze reviews,we implemented and compared three types of linear classifiers: 
the Perceptron Algorithm, the Average Perceptron Algorithm, and the Pegasos Algorithm.


project1.py contains various useful functions and function templates that you will use to implement your learning algorithms.
main.py is a script skeleton where these functions are called and you can run your experiments.
utils.py contains utility functions that the staff has implemented for you.
test.py is a script which runs tests on a few of the methods you will implement. Note that these tests are provided to help you debug your implementation and are not necessarily representative of the tests used for online grading. Feel free to add more test cases locally to further validate the correctness of your code before submitting to the online graders in the codeboxes.

In this project we implemented linear classifiers beginning with the Perceptron algorithm. 
we began by defining loss function, a hinge-loss function and then total Hinge loss function.
we then defined Perceptron , Average Perceptron and Perceptron algorithms and found their training and validation accuracies.
Based on the accuracy, a model is selected and is applied for test dataset. Finally using parameter tuning, we have selected best values for the parameters iterations(T) and learning rate(L).
In the currect project, we've used Bag of Words approach to tokenize and build vocabulary and also
based on selected stopwords, we tried to increase the accuracy of our model. 


## Parameter Tuning for Pegasos Algorithm

![App Screenshot](https://raw.githubusercontent.com/AbhinavGavireddi/Machine-Learning-projects/main/sentiment_analysis/Parameter%20tuning%20results/Figure%202022-06-15%20231825%20(2).png?token=GHSAT0AAAAAABVU4TFVFRB62BQ7MPJA3Y72YVKFISA)

![App Screenshot](https://raw.githubusercontent.com/AbhinavGavireddi/Machine-Learning-projects/main/sentiment_analysis/Parameter%20tuning%20results/Figure%202022-06-15%20231825%20(3).png?token=GHSAT0AAAAAABVU4TFU24N4FQRTBZAWP7JWYVKFKDA)