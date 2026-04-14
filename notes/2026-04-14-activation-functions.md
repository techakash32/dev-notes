# Activation Functions
=====================================

## Learning Objective

* Understand the concept of activation functions in neural networks
* Learn about different types of activation functions and their properties
* Be able to choose the right activation function for a given problem
* Implement activation functions in a neural network

## Concept Explanation

### What are Activation Functions?

Activation functions are a crucial component of neural networks. They are used to introduce non-linearity into the model, allowing it to learn and represent more complex relationships between inputs and outputs. Without activation functions, neural networks would be limited to learning linear relationships, which is not sufficient for most real-world problems.

### Why Do We Need Activation Functions?

The main reason we need activation functions is to introduce non-linearity into the model. This is because most real-world problems are non-linear in nature, and a linear model would not be able to capture these relationships. Additionally, activation functions help to avoid the problem of vanishing gradients, which occurs when the gradients used to update the model's weights become very small during backpropagation.

### Types of Activation Functions

There are several types of activation functions, each with its own strengths and weaknesses. Some of the most common activation functions are:

#### 1. Sigmoid

The sigmoid activation function maps the input to a value between 0 and 1. It is often used in the output layer of a binary classification problem, where the output is a probability.

$$\sigma(x) = \frac{1}{1 + e^{-x}}$$

#### 2. ReLU (Rectified Linear Unit)

The ReLU activation function is a simple and computationally efficient function that maps all negative values to 0 and all positive values to the same value.

$$f(x) = \max(0, x)$$

#### 3. Tanh (Hyperbolic Tangent)

The tanh activation function maps the input to a value between -1 and 1. It is similar to the sigmoid function, but the output range is larger.

$$	anh(x) = \frac{e^x - e^{-x}}{e^x + e^{-x}}$$

#### 4. Softmax

The softmax activation function is often used in the output layer of a multi-class classification problem, where the output is a probability distribution.

$$\sigma(x)_i = \frac{e^{x_i}}{\sum_{j=1}^n e^{x_j}}$$

#### 5. Leaky ReLU

The leaky ReLU activation function is a variation of the ReLU function that allows a small fraction of the input to pass through, even if it is negative.

$$f(x) = \max(\alpha x, x)$$

#### 6. Swish

The swish activation function is a recently introduced function that has been shown to be more effective than ReLU and other activation functions in some cases.

$$f(x) = x \cdot g(x)$$

where $g(x)$ is a learnable function.

### Key Concepts

* **Non-linearity**: Activation functions introduce non-linearity into the model, allowing it to learn and represent more complex relationships between inputs and outputs.
* **Vanishing gradients**: Activation functions help to avoid the problem of vanishing gradients, which occurs when the gradients used to update the model's weights become very small during backpropagation.
* **Computational efficiency**: Some activation functions, such as ReLU, are computationally efficient and can speed up the training process.

### Comparison Tables

| Activation Function | Output Range | Computational Efficiency | Non-Linearity |
| --- | --- | --- | --- |
| Sigmoid | (0, 1) | Low | High |
| ReLU | (0, ∞) | High | Low |
| Tanh | (-1, 1) | Medium | High |
| Softmax | (0, 1) | Low | High |
| Leaky ReLU | (0, ∞) | High | Medium |
| Swish | (-∞, ∞) | Medium | High |

### Real-World Examples

* **Image classification**: ReLU and its variants are often used in image classification problems, where the output is a probability distribution over multiple classes.
* **Natural language processing**: Sigmoid and softmax are often used in natural language processing problems, where the output is a probability distribution over multiple classes.
* **Recommendation systems**: Tanh and ReLU are often used in recommendation systems, where the output is a rating or a probability.
* **Game playing**: Swish and ReLU are often used in game playing, where the output is a probability distribution over multiple actions.
* **Robotics**: Leaky ReLU and ReLU are often used in robotics, where the output is a control signal.

### Cheat Sheet

| Activation Function | Formula | Output Range |
| --- | --- | --- |
| Sigmoid | σ(x) = 1 / (1 + e^(-x)) | (0, 1) |
| ReLU | f(x) = max(0, x) | (0, ∞) |
| Tanh | tanh(x) = (e^x - e^(-x)) / (e^x + e^(-x)) | (-1, 1) |
| Softmax | σ(x)_i = e^(x_i) / Σ e^(x_j) | (0, 1) |
| Leaky ReLU | f(x) = max(αx, x) | (0, ∞) |
| Swish | f(x) = x \* g(x) | (-∞, ∞) |

### Interview Questions

1. What is the purpose of activation functions in neural networks?
2. What are the different types of activation functions?
3. What is the sigmoid activation function, and when is it used?
4. What is the ReLU activation function, and when is it used?
5. What is the tanh activation function, and when is it used?
6. What is the softmax activation function, and when is it used?
7. What is the leaky ReLU activation function, and when is it used?
8. What is the swish activation function, and when is it used?
9. How do activation functions introduce non-linearity into the model?
10. How do activation functions help to avoid the problem of vanishing gradients?

### Practice Exercises

1. Implement the sigmoid activation function in Python.
2. Implement the ReLU activation function in Python.
3. Implement the tanh activation function in Python.
4. Implement the softmax activation function in Python.
5. Implement the leaky ReLU activation function in Python.

### Solutions

1. `def sigmoid(x): return 1 / (1 + np.exp(-x))`
2. `def relu(x): return np.maximum(0, x)`
3. `def tanh(x): return np.tanh(x)`
4. `def softmax(x): return np.exp(x) / np.sum(np.exp(x))`
5. `def leaky_relu(x, alpha=0.01): return np.maximum(alpha * x, x)`

### Summary

Activation functions are a crucial component of neural networks, introducing non-linearity into the model and helping to avoid the problem of vanishing gradients. There are several types of activation functions, each with its own strengths and weaknesses. The choice of activation function depends on the specific problem and the desired output. In this note, we have covered the concept of activation functions, different types of activation functions, key concepts, comparison tables, real-world examples, a cheat sheet, interview questions, practice exercises, and a summary.