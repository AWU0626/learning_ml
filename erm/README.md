# What is Empirical Risk Minimization (ERM)?

In machine learning, we task the machine (the learner) with making a correct prediction on any unseen datum. The process of machine learning, as the name suggests, is to design a way for the machine to learn and predict results better.

The process revolves around a dataset $D$, consisting of datapoints $d$. Each datapoint contains a set of features $x$ and a label $y$ that we want to predict. We then use a subset of $D$, the training data, for our learner to learn from, and evaluate its performance on a different subset of $D$, the testing data.

Empirical Risk Minimization (ERM), in the context of learning, is the paradigm that focuses on reducing the prediction error that our learner has after being trained on the training data.

For a more detailed overview, see Chapter 2 of *Understanding Machine Learning: From Theory to Algorithms* ([free PDF](https://www.cs.huji.ac.il/~shais/UnderstandingMachineLearning/copy.html)).
