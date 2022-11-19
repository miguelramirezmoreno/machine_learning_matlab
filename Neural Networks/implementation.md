# Neural Networks

## Cost function

It now is a generalization of the cost function for logistic regression, but now applied to

<img width="677" alt="image" src="https://user-images.githubusercontent.com/43887905/201468116-980bf603-795d-4292-8e02-52c47bb583cd.png">

```math
J(\theta)= - \frac{1}{m}  \left[ \sum_{i=1}^m y^{(i)} \log(h_\theta(x^{(i)}) + (1-y^{(i)})\log(h_\theta(x^{(i)}  \right] + \frac{\lambda}{2m} \left[ \sum_{j=1}^n \theta^2_j \right]
```


### Cost function for neural network:

<img width="848" alt="image" src="https://user-images.githubusercontent.com/43887905/201468106-34f765ad-896f-428c-9d06-c37bb101667b.png">

```math
h_\Theta(x) \in R^K 
```
```math
J(\Theta)= - \frac{1}{m}  \left[ \sum_{i=1}^m y^{(i)} \log(h_\theta(x^{(i)}) + (1-y^{(i)})\log(h_\theta(x^{(i)}  \right] + \frac{\lambda}{2m} \left[ \sum_{j=1}^n \theta^2_j \right]

```

```
code
```
### Backpropagation algorythm.

Aims to reduce the cost function in NN. Forward propagation is what allows us to compute the output of the NN. The error of node j in layer l is represented as delta^{(l)}j. The error is the output [ a(l)j - yj

```
deltatotal= 0;
for i = 1:m
   set a(1) = x(i)
   compute a(l) with forward propagation
   compute delta(L) as= a(L) -y(i), then detla (L-1)... up to      delta(2)
   Deltatotal_ij(l) := Deltatotal_ij(l) + a_j(l)*delta_i(l+1)
   ```
   
   <img width="338" alt="image" src="https://user-images.githubusercontent.com/43887905/201470193-06d24e62-e276-46ac-b20b-cceb74d0902e.png">

   
Aims to reduce the cost function in NN. Forward propagation is what allows us to compute the output of the NN. The error of node j in layer l is represented as delta^{(l)}j. The error is the output [ a(l)j - yj
