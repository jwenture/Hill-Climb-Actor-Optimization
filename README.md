# Hill Climb Actor Optimization
Gradient Descent policy estimators are slow to converge and are highly susceptible to initializations. 
We present a different optimization method that utilizes random hill search and Advantage-Actors to quickly find optimal solutions.

While we can shift to A3C/A2C/PPO models to fully optimize solutions eventually, the initial learning steps can be extremely slow.
Instead of gradient descent through backpropagation, we will directly alter the weights of each layer based on normalized returns.
We can bypass the vanishing gradient problem since the neuron weight changes are independent (or slightly dependent) from the weights. 
