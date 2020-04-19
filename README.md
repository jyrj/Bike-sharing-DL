![Deep Learning Nanodegree Project 1](bike-sharing-cover.jpg)
# Bike-Sharing-Pattern-with-NeuralNet
Developed as coursework for Udacity ```"Deep Learning Nanodegree"```.
In this project, I built a neural network to predict daily bike rental ridership.

## Further Explanation
The Neural network was built from "scratch", using only NumPy to assist. The goal of this project is to understand what happens behind the neural network before diving deeper into other tools like TensorFlow.

## Results
The project meets the specifications, which are:
- All the code in the notebook runs in Python 3 without failing, and all unit tests pass.
- The sigmoid activation function is implemented correctly
- The forward pass is correctly implemented for the network's training.
- The run method correctly produces the desired regression output for the neural network.
- The network correctly implements the backward pass for each batch, correctly updating the weight change.
- Updates to both the input-to-hidden and hidden-to-output weights are implemented correctly.
- The number of epochs is chosen such the network is trained well enough to accurately make predictions but is not overfitting to the training data.
- The number of hidden units is chosen such that the network is able to accurately predict the number of bike riders, is able to generalize, and is not overfitting.
- The learning rate is chosen such that the network successfully converges, but is still time efficient.
- The number of output nodes is properly selected to solve the desired problem.
- The training loss is below 0.09 and the validation loss is below 0.18.

## Code comments from Udacity reviewer
All functions were implemented correctly, and the final algorithm seems to work quite well.
- The sigmoid activation function was correctly implemented.
- Be careful, because an excessive number of iterations (epochs) can cause overfitting.
- You should avoid using learning rates lower than enough to get the network to converge.
- Udacity suggests using at least 8 hidden nodes in this project.
- Be careful, because an excessive number of hidden nodes can cause overfitting.

## Conclusion
The predictions given by the model are quite accurate. However, the model overestimes bike ridership in December because it hasn't had sufficient holiday season training examples.

## Observed Errors

On the original Predicting_bike_sharing_data.ipynb, it will show ```DataFrame'object has no attribute ix```. In order to avoid that error message, you can switch to older pandas version. Type the below the line of code on to your jupyter notebook cell to install older pandas;
    
    !pip install pandas==0.25.1
 or you could continue using the same Pandas in .ipynb with replaced usage of ```iloc```
 
Author: [Jayaraj J](https://www.linkedin.com/in/jyjnair)

[You can find me here](jyrj.github.io)