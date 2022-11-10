# Neural Networks

## Cost function

It now is a generalization of the cost function for logistic regression, but now applied to
```math
J(\theta)= - \frac{1}{m}  \left[ \sum_{i=1}^m y^{(i)} \log(h_\theta(x^{(i)}) + (1-y^{(i)})\log(h_\theta(x^{(i)}  \right] + \frac{\lambda}{2m} \left[ \sum_{j=1}^n \theta^2_j \right]
```


### Cost function for neural network:
```math
h_\Theta(x) \in R^K 
```
```math
J(\Theta)= - \frac{1}{m}  \left[ \sum_{i=1}^m y^{(i)} \log(h_\theta(x^{(i)}) + (1-y^{(i)})\log(h_\theta(x^{(i)}  \right] + \frac{\lambda}{2m} \left[ \sum_{j=1}^n \theta^2_j \right]

```
