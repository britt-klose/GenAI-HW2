# GenAI-HW2: Comparing MLP & CNN Architectures 

**Overview:**
This assignment compares the performance of a simple Multi-Layer Perceptron (MLP) and a Convolutional Neural Network (CNN) using strides on the CIFAR-10 dataset.

# Discussions Points

**Performance Comparison:**
The MLP model showed decreases in loss and increases in accuracy with each epoch. However, the final product was still very low in accuracy and high in loss. In comparison for the CNN model the accuracy was much higher. In MLP the highest accuracy was around 0.44 and the highest accuracy for the CNN model was around 0.78. More so, the accuracy for CNN increased about 0.4 from the first epoch to the 10th. Whereas in the MLP model the increase in accuracy only jumped about 0.2 from the first epoch to the 10th. Additionally, the loss for MLP was significantly higher than in the CNN model and decreased very little and much less than the CNN. To elaborate, the loss for the MLP model began around after the first epoch and ended around 1.9 and ended around 1.56. Versus in the CNN model the loss went from 1.8 to about 0.6. Overall, this demonstration has emphasized that CNNs perform much better for image classification. 

**Model Complexity:**
The main issue with MLPs is that they don’t consider the spatial structure of images in the input. Whereas CNNs with their convolutional layers can capture the higher level features by flattening images into a single vector that can be processed by the first dense layer. This is done by multiplying the filter pixelwise with a portion of the image and summarizing the results. 

**Training Time:**
The computation time for the CNN model was about 1 minute and 40 seconds and it was about 1 minute 11 seconds for the MLP model. The slightly shorter time for the MLP model was expected as CNNs include more layers and are more complicated in order to capture the high level features. 

**Overfitting & Regularization:**
Propagation can be helped by regularization techniques that ensure models don’t overfit. Having drop out layers is the most common regularization technique and is typically used after dense layers since they’re most likely to be victim to overfitting. Dropout layers decrease chance of overfitting by ensuring that the network is not dependent on certain units, ie. just memorizing things from its training. Instead the model makes observations from its training and learns from them. Thus, the network will be trained to produce more accurate guesses even when undergoing new conditions. 
