# Double_Descent_Phenomenon
Observing the double descent Phenomenon occurring in over parametrized models such as Deep Neural Networks 

With few parameters to learn, the model tends to have high bias (underfitting) and low variance, while a complex model with many parameters tends to have low bias and high variance (overfitting).

Thus, the ultimate goal in supervised machine learning is to find a model with an optimal balance 
between bias and variance that can generalize well to new unseen data.
Traditional statistical mindset from the bias-variance tradeoff indicates that simpler models with
fewer parameters should be more performant than complex models with many parameters.

However, recent experiments have proven that interpolators-estimators that achieve zero training
error such as deep neural networks which often have large number of parameters to learn compared
to the size of the dataset, achieve a good generalization performance than simple models with
few parameters. This behavior is known in terms of a so-called "double-descent" curve, and this
seems at first to defy the traditional statistical mindset. It has been conjectured that the good
generalization behavior in this highly overparametrized regime is due to the implicit regularization
induced by gradient descent learning. [20] Since Neural Networks use gradient descent learning
algorithm, one could think that this double descent behavior in Neural Networks is due to the
gradient Descent Learning. However, some experiments have been made using linear model
`ridgeless least square regression' in an overparametrized regime and the authors have observed
this `double descent' curve. And it turns out that the optimum performance of the generalization
error is achieved in the overparametrized regime, beyond the interpolation threshold.
In this work, we do two experiments and we observe the "double descent" curve. 

One experiment using a linear model and the second one using a linear model together with a nonlinear activation
function, which has been proved in some Machine learning research papers to have a direct connection with
complex models such as neural networks, emphasizing that in certain overparametrized settings,
linear models provide more than a simple analogy to Neural Networks.

We give some settings for this phenomenon to be observed and we give the intuitive explanation
behind.
