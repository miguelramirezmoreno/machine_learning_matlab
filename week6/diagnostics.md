# Diagnostic

When the model does not fit a new training set. What do we do? Add parameters? Reduce parameters? Polynomial? Changing Lambda? This can be very time consuming if we want to evaluate everything.

Evaluation consists in separating training sets in two groups, "training set" and "test set" (usually 70-30% of the total dataset). So training set mecomes *m* and m_training. We use training data to learn new parameters, and we compute the error of the new parameters in the test set. (J_subtest(theta). with the basic cost function., or in the case of logistic regression:

<img width="833" alt="image" src="https://user-images.githubusercontent.com/43887905/202869931-e187ac61-2e4d-4794-b654-be09530fee82.png">

Alternativelly, we can use the misclassification error, or (0/1 error). 
