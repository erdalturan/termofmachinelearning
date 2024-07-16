Bayesin optimization is a powerful method for optimizing black-box functions. Here are the key parameters and a brief description:
**Parameters:**
1. **Initialization**: The initial points to start the optimization process. This is usually a set of random points in the search space.
2. **Acquisition function**: A function that determines the next point to evaluate based on the current model of the objective function. Common acquisition functions include:
* Probability of Improvement (PI)
* Expected Improvement (EI)
* Upper Confidence Bound (UCB)
* Entropy Search (ES)
3. **Surrogate model**: A probabilistic model that approximates the objective function. Common surrogate models include:
* Gaussian Process (GP)
* Random Forest (RF)
* Neural Networks (NN)
4. **Objective function**: The function to be optimized.
5. **Search space**: The domain of the objective function.
6. **Iteration budget**: The number of iterations (evaluations of the objective function) allowed.
7. **Kernel**: A function that computes the covariance between points in the search space. Common kernels include:
* Radial Basis Function (RBF)
* Matérn kernel
* Exponential kernel
**Description:**
Bayesian optimization involves the following steps:
1. **Initialization**: Initialize the surrogate model with the initial points.
2. **Acquisition**: Choose the next point to evaluate using the acquisition function.
3. **Evaluation**: Evaluate the objective function at the chosen point.
4. **Update**: Update the surrogate model with the new evaluation.
5. **Repeat**: Repeat steps 2-4 until the iteration budget is exhausted.
6. **Optimum**: Return the point with the best objective function value as the optimum.
The key idea behind Bayesian optimization is to model the objective function using a probabilistic surrogate model, which allows us to quantify the uncertainty in the function values. The acquisition function then uses this uncertainty to select the next point to evaluate, balancing exploration and exploitation.
Bayesian optimization is particularly useful when the objective function is expensive to evaluate, noisy, or has multiple local optima.



# Grid search
   In grid search, we first start by defining a grid containing the list of hyperparameters along with lists of acceptable values you would want the search process to try. Following is a sample    hyperparameter grid for a Logistic Regression model:   
   
# Random search
In random search, other than defining a grid of hyperparameter values, we specify a distribution from which the acceptable values for the specified hyperparameters could be sampled. The main difference between random search and grid search is that instead of trying all the possible combinations of hyperparameters, each combination of hyperparameters is sampled randomly and the hyperparameter values come from the distribution that we specify at the beginning of the random search process.

# Define Hyperparameters Keys

    LEARNING_RATE = 'Learning Rate'
    MAX_EPOCHS = 'Max Epochs'
    BATCH_SIZE = 'Batch Size'
    HIDDEN_LAYERS = 'Hidden Layers'
    LOSS_FUNCTION = 'Loss Function'
    ACTIVATION_FUNCTION = 'Activation Function'
    OPTIMIZER = 'Optimizer'
    DROPOUT = 'Dropout'
    L1_REGULARIZATION = 'L1 Regularization'
    L2_REGULARIZATION = 'L2 Regularization'
    WEIGHT_INITIALIZATION = 'Weight Initialization'
    LSTM_NUMBER_OF_LAYERS = 'Number of Layers'
    LSTM_HIDDEN_LAYER_SIZE = 'Hidden Layer Size'
