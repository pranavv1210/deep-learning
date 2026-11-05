# Mathematics for Deep Learning

This is a practical companion to the deep-learning notebooks. Each mathematical idea is introduced because it appears in neural-network computation.

## 1. Vectors, matrices and tensors

A vector is a one-dimensional collection of numbers. A matrix is a two-dimensional table. A tensor generalizes this idea to any number of dimensions.

Common examples:
- Scalar loss: shape `()`
- Batch of 32 feature vectors with 10 features each: shape `(32, 10)`
- Batch of 8 grayscale 28×28 images in channels-last format: shape `(8, 28, 28, 1)`

A tensor's **shape** describes its dimensions. Its **dtype** describes the number representation, such as integer or float32. A **batch dimension** identifies how many examples are processed together.

## 2. Weighted sums and neurons

A basic neuron calculates:

`z = w1*x1 + w2*x2 + ... + wn*xn + b`

The x values are inputs, w values are weights, and b is a bias. The neuron then applies an activation function:

`a = activation(z)`

Weights control how strongly inputs contribute. Bias shifts the weighted sum. Activation functions allow networks to represent non-linear relationships.

## 3. Matrix multiplication

For a batch of inputs X and a weight matrix W, a layer often computes:

`Z = XW + b`

The dimensions must match: if X has shape (batch_size, input_features), W has shape (input_features, output_units), then Z has shape (batch_size, output_units).

Always write down shapes when a matrix multiplication error occurs.

## 4. Derivatives and the chain rule

A derivative tells how sensitive an output is to a small change in an input. A neural network is a chain of functions, so the chain rule lets us calculate how the final loss depends on an earlier parameter.

For functions y=f(u) and u=g(x):

`dy/dx = (dy/du) * (du/dx)`

Backpropagation applies this principle efficiently from the output layer back toward earlier layers.

## 5. Gradient descent

Let L be the loss and w a trainable parameter:

`w_new = w_old - learning_rate * (dL/dw)`

The gradient indicates the direction of increasing loss, so we subtract it to move toward lower loss. Learning rate controls the update size.

## 6. Common losses

- **Mean squared error (MSE):** average squared difference between numeric predictions and targets. Large errors receive a stronger penalty because errors are squared.
- **Binary cross-entropy:** measures the mismatch between predicted probabilities and binary labels.
- **Categorical cross-entropy:** commonly used when a model predicts a probability distribution over multiple classes.

The output activation and loss must be chosen consistently with the task and label format.

## 7. Convolution intuition

A convolutional filter is a small grid of learned weights that slides across an image. At each position it combines nearby pixels to produce a feature response. Early layers may respond to edges and textures; deeper layers can combine them into more complex patterns.

- **Kernel/filter:** the small learned weight grid.
- **Stride:** how far the filter moves each step.
- **Padding:** extra border values added to control spatial output size.
- **Feature map:** the output produced by applying a filter.

## 8. Attention intuition

Attention lets a token build a representation by weighing information from other tokens. Queries express what a token is looking for; keys describe candidate information; values carry the information to combine. Similarity scores are normalized into weights and used to form a weighted sum.

Read the Transformers chapter for the full scaled dot-product attention formula and a worked example.

## More resources
- [3Blue1Brown neural networks](https://www.3blue1brown.com/topics/neural-networks)
- [Dive into Deep Learning](https://d2l.ai/)
