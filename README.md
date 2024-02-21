# Handwriting Classification with a Convolutional Neural Network

I wanted to write and implement a convolutional neural network using PyTorch that would be able to classify handwriting data using a train, valid, test approach. The following shows my exploration and process to implement this successfully. This was a fun exercise, and I got to learn a lot more about convolutional neural networks. I hope you enjoy!

## Contents

1. [Numerical Handwriting Classification](#1-numerical-handwriting-classification)

## 1. Numerical Handwriting Classification

### 1.1 Data
<img width="149" alt="image" src="https://github.com/austinfroste/handwriting_classification_cnn/assets/65328557/846a485b-b016-4f25-a276-2158a53ad270">

<em>**Figure 1. Torchvision MNIST Dataset**</em>

I used the Torchvision [MNIST Dataset](https://pytorch.org/vision/stable/generated/torchvision.datasets.MNIST.html#torchvision.datasets.MNIST) for my model (sample seen above). The data consists of grayscale images of handwritten single digit numerical characters in the range 0 through 9. This dataset is from the MNIST (Modified National Institute of Standards and Technology) and is highly coveted as a machine-learning-friendly human handwriting dataset. To learn a little more about the dataset, [see more](https://en.wikipedia.org/wiki/MNIST_database).


### 1.2 Model
I implemented a convolutional neural network with two hidden layers, L2 norm regularization, and a learning rate of 0.001 and got the following results. You can view the deployed model in a Jupyter Notebook [here](numeric_handwriting.ipynb).

### 1.3 Results
I will now present the results of my model:

<img width="691" alt="image" src="https://github.com/austinfroste/handwriting_classification_cnn/assets/65328557/3fe49552-a5d9-4e3c-8568-fba6c7b2b482">

<em>**Figure 2. Model Output**</em>

<img width="848" alt="image" src="https://github.com/austinfroste/handwriting_classification_cnn/assets/65328557/f31378ec-bfdb-4265-a3a8-c64ca58408ca">

<em>**Figure 3. Prediction Accuracy Performance**</em>

<img width="854" alt="image" src="https://github.com/austinfroste/handwriting_classification_cnn/assets/65328557/718003e8-c5bf-4024-b287-15f1370f2ce9">

<em>**Figure 4. Prediction Loss Performance**</em>

### 1.4 Findings
My model boasted test high accuracy that converged around 98 to 99 percent (Figure 2). This high test accuracy was coupled with low test loss that converged at around 0.025 to 0.035 (Figure 2). My model performed well on the unseen test and valid data, as seen in both accuracy and loss curves (Figures 3, 4), further showing the success of the model.

### 1.5 Next steps
Seeing that I was able to implement a successful model using numerical data, I would now like to further expand into more complex data such as alphabetical.

---

Thanks for checking out my project!
