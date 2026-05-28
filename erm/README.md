# What is Empirical Risk Minimization (ERM)?

In machine learning, we task the machine (the learner) with making a correct prediction on any unseen datum. The process of machine learning, as the name suggests, is to design a way for the machine to learn and predict results better.

The process revolves around a dataset $\mathcal{D}$, consisting of datapoints $d$. Each datapoint contains a set of features $x$ and a label $y$ that we want to predict. We then use a subset of $S\subseteq \mathcal{D}$, the training data, for our learner to learn from, and evaluate its performance.

Empirical Risk Minimization (ERM), in the context of learning, is the paradigm that focuses on reducing the prediction error that our learner has after being trained on the training data, i.e. minimizing training error.

In essence, we want our learner to adapt some hypothesis in a set of all hypotheses $h\in \mathcal{H}$, (a model amongst the set of all learning models) that would reduce the prediction error of our learner.

Formally we would define the following:

$
\mathcal{H}: \text{the set of all models} \\
\mathcal{S}: \text{the set of training data used for out learner} \\ 
ERM_{\mathcal{H}}(S): \text{the model that minimizes risks} \\
L_{S}(h): \text{our learner trained using } S \text{ using the model } h \\
$

and our objective is to find the model $h$ that minimizes risk. Formally, this becomes:

$$
ERM_{\mathcal{H}}(S) = \argmin_{h\in \mathcal{H}} L_{S}(h)
$$

For a more detailed overview, see Chapter 2 of *Understanding Machine Learning: From Theory to Algorithms* ([free PDF](https://www.cs.huji.ac.il/~shais/UnderstandingMachineLearning/copy.html)).
