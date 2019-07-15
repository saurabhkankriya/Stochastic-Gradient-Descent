# Stochastic-Gradient-Descent
Implementing SGD from scratch for linear regression

**Gradient Descent** is computational technique that is used to find minima and maxima without solving differential equations. It is an interative algorithm. Make a random guess of w0. then do a random guess of w1 at iteration 1 and so on till iteration k which is very close to W*

1. In gradient descent you consider all the data points to update your weights
2. In stochastic gradient descent you use k(it can be as low as 1 data point) random data points to update your weights(computationally more efficient).


In logistic/linear regression and linear SVMs, the cost function is generally convex(i.e. there can exist only one minima) and hence there will only be one minima. In the case of neural nets, the cost function is generally non-convex(as there can exist multiple minima).

What we are trying to achieve is to find best slope and intercept for our line that best fits our data. So its basically an optimisation technique. Here we are initiating by taking slope and intercept=0 than calculating error in each step and then updating slope & intercept accordingly till we reach best fit. For slope, gradient is used that gives us minima means point that gives best slope and intercept with min error.

If local minima and global minima are different, gradient descent is not guaranteed to converge to global minima. Whether grad-descent reaches global or local optima depends on the initial point (x_0). So we can try various initial points, run the grad-descent, obtain multiple minima and pick the best one at the end.

**Learning Rate:**  By decaying or reducing the learning rate you try to move as near to the local minima as possible. By increasing the learning rate performance will diverge. You would notice that the loss number jump to extremely high levels until it becomes NAN . This happens because the gradient is only a good approximation of the loss function in the local space . When your learning rate is too high, you are taking huge steps, and most likely you’d miss the minima. This is the classic divergence scenario.




**Summary:**
1. May have Maxima and Minima .
2. Could have only minima .
3. May not have both Maxima and Minima.
4. Multiple Minima Multiple Maxima.
5.Could have only Maxima .
6. Can have multiple local maximas, minimas but only one global Maxima or global minima.
7. df/dx=0 doesn’t work always ! Gradient Descent is the solution.
