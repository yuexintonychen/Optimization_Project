## Optimization Project: Lookahead Optimizer
Absctract:

Micheal Zhang from University of Toronto discovered a new method of optimization, called 
Lookahead(https://arxiv.org/pdf/1907.08610). This optimization method can utilize any optimization method as the backbone. 
In this project, we did a comparison test on this optimization method on the top layer, with other widely used optimization 
methods, such as Adam, SGD and Gradient Descent to verify whether the Lookahead optimization method can improve convergence 
as Micheal stated in his paper. 

Based on what we get from implementing the Lookahead optimization method on simple optimization problem and neural network, 
we find that we have different outcomes with the original paper. First of all, we do not see that the improvement of 
convergence is a general situation, that is it does not mean that it is necessary to apply the Lookahead optimization method 
over any standard optimization methods. We conclude that the Lookahead optimization method can somehow improve the convergence 
but for some specific backbone optimizers, parameters, nets if using neural networks and datasets. And there is one problem 
we find during the coding, the original paper does not states whether initialize the backbone optimizer for each step of the 
Lookahead or we continue using the states from the previous one. This can make a difference on running Lookahead, and it still 
needs to be tested out.
