## Udacity_DeepLearning_Google
Homework and notes for Udacity Deep learning courses

###Basic concept

**One-Hot encoding**
In multi-class classification problem, encode the true class 1 and all else 0. Same as one-vs-all encoding


**Cross-entropy**
D(S,L) = -Sum(S*log(L)) #L stands for labels and S stands for distribution
D(S,L) != D(L,S) not symmetric

Feature scaling for images. Since pixels have a range (0,255), use (value-128)/128 to scale them.

**ReLU**
Rrectified linear unit. It is the activation function. Defined as: h=max(0,a) where a=Wx+b
[What is ReLU](https://en.wikipedia.org/wiki/Rectifier_(neural_networks))

Compare to sigmoid function, two additional major benefits of ReLUs are sparsity and a reduced likelihood of vanishing gradient. 

1. One major benefit is the reduced likelihood of the gradient to vanish. This arises when a>0. In this regime the gradient has a constant value. In contrast, the gradient of sigmoids becomes increasingly small as the absolute value of x increases. The constant gradient of ReLUs results in faster learning.

2. The other benefit of ReLUs is sparsity. Sparsity arises when a≤0. The more such units that exist in a layer the more sparse the resulting representation. Sigmoids on the other hand are always likely to generate some non-zero value resulting in dense representations. Sparse representations seem to be more beneficial than dense representations.


###Further reading

**Compare two images**
[Very detailed tech from StackOverflow](http://stackoverflow.com/questions/189943/how-can-i-quantify-difference-between-two-images)

**Intercept of logistic regerssion**
[About interpretation about fit intercept or not](http://stats.stackexchange.com/questions/131456/confused-about-0-intercept-in-logistic-regression-in-r)

###Assignment 1

