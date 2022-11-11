## Requirements



## Cost Function for multiple variables

``
function J = cost_lrm(X, y, theta)

m = length(y);
J = 0;
``


## Gradient descent multiple variables

``
function [theta, J_history] = gradientdescentlrm(X, y, theta, alpha, num_iters)

m = length(y);

J_history = zeros(num_iters, 1);

for iter = 1:num_iters
    theta = theta - alpha / m *  X' * (X * theta - y);
        J_history(iter) = computeCostMulti(X, y, theta);
        end

end

``
