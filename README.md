# handwriting_classification_cnn

I wanted to write and implement a convolutional neural network using PyTorch that would be able to classify handwriting data using a train, valid, test approach. The following shows my exploration and process to implement this successfully.

## Contents

1. [Numerical Handwriting Classification](#1-numerical-handwriting-classification)

## 1. Numerical Handwriting Classification

### 1.1 Data
<img width="149" alt="image" src="https://github.com/austinfroste/handwriting_classification_cnn/assets/65328557/846a485b-b016-4f25-a276-2158a53ad270">

I used the Torchvision [MNIST dataset](https://pytorch.org/vision/stable/generated/torchvision.datasets.MNIST.html#torchvision.datasets.MNIST) for my model (sample seen above). The data consists of grayscale images of handwritten single digit numerical characters in the range 0 through 9. This dataset is from the MNIST (Modified National Institute of Standards and Technology) and is highly coveted as a machine-learning-friendly human handwriting dataset. To learn a little more about the dataset, [see more](https://en.wikipedia.org/wiki/MNIST_database).


### 1.2 Model
I implemented a convolutional neural network with two hidden layers, L2 norm regularization, and a learning rate of 0.001 and got the following results. You can view the deployed model in a Jupyter Notebook [here](handwriting_classification_cnn.ipynb).

### 1.3 Results
The output for my model is as follows:

<img width="698" alt="image" src="https://github.com/austinfroste/handwriting_classification_cnn/assets/65328557/2bcd9f3d-1ec8-4e24-93f0-ed91f45c76f1">
<img width="854" alt="image" src="https://github.com/austinfroste/handwriting_classification_cnn/assets/65328557/414b8a75-f2d6-473e-98f4-784a6751901b">
<img width="869" alt="image" src="https://github.com/austinfroste/handwriting_classification_cnn/assets/65328557/67254d54-efbd-424a-ad4d-2f6747643c5b">

### 1.4 Findings
My model boasted test high accuracy that converged around 98 to 99 percent. This high test accuracy was coupled with low test loss that converged at around 0.025 to 0.035. My model performed well on the unseen test and valid data, as seen in both accuracy and loss curves, further showing the success of the model.
