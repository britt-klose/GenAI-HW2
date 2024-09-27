# GenAI-HW2: Comparing MLP & CNN Architectures 

**Overview:**
This assignment compares the performance of a simple Multi-Layer Perceptron (MLP) and a Convolutional Neural Network (CNN) using strides on the CIFAR-10 dataset.

# Discussions Points

**Performance Comparison:**

**Model Complexity:**
The main issue with MLPs is that they don’t consider the spatial structure of images in the input. Whereas CNNs with their convolutional layers can capture the higher level features by flattening images into a single vector that can be processed by the first dense layer. This is done by multiplying the filter pixelwise with a portion of the image and summarizing the results. 

**Training Time:**

**Overfitting & Regularization:**
Propagation can be helped by regularization techniques that ensure models don’t overfit. Having drop out layers is the most common regularization technique and is typically used after dense layers since they’re most likely to be victim to overfitting. Dropout layers decrease chance of overfitting by ensuring that the network is not dependent on certain units, ie. just memorizing things from its training. Instead the model makes observations from its training and learns from them. Thus, the network will be trained to produce more accurate guesses even when undergoing new conditions. 
