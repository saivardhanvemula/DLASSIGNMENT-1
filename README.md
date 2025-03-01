# DLASSIGNMENT-1

Key Observations:
Adam optimizer consistently outperformed other optimizers (e.g., SGD, Momentum) in terms of both speed and accuracy due to its adaptive learning rate.
ReLU activation was the most effective, as it avoided the vanishing gradient problem and facilitated faster convergence. Sigmoid struggled, especially in deeper networks.
Adding more hidden layers and neurons improved performance to a point but caused overfitting beyond 4 layers and 64 neurons.
A learning rate of 1e-3 was ideal for most optimizers, providing the best convergence speed without instability.
Weight decay (L2 regularization) at 0.0005 helped prevent overfitting, but larger values led to poor performance.
Batch size of 32 worked well for balancing training time and model performance.
Best Performing Configuration:
Optimizer: Adam
Activation: ReLU
Hidden Layers: 3-4 layers
Neurons per Layer: 64
Batch Size: 32
Learning Rate: 1e-3
Recommendations for MNIST:
Based on these results, the following configurations are recommended for MNIST:

Use Adam optimizer with ReLU activation.
Set the learning rate to 1e-3.
Use 3-4 hidden layers with 64 neurons per layer to avoid overfitting while ensuring good performance.
