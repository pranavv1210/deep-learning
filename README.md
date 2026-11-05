# Deep Learning — A Practical Study Path

This repository teaches deep learning step by step, from tensor operations and neural-network fundamentals to computer vision, sequence models, transformers, generative models, evaluation and deployment.

The original 33 numbered learning areas, project notebooks, data files and existing outputs are retained. The notebooks should be studied in order, with particular care given to the mathematical intuition and the meaning of each training result.

## Recommended learning sequence

| Stage | Chapters | What you learn |
|---|---|---|
| Python and data tools | 01–04 | Python, NumPy, Pandas, plotting |
| Neural-network foundations | 05–13 | Tensors, neurons, activations, loss, optimizers, gradients, ANN |
| Frameworks | 14–16 | TensorFlow, Keras, PyTorch |
| Vision | 17–20 | Image tensors, CNNs, transfer learning, augmentation |
| Sequences and language | 21–25 | RNN, LSTM, GRU, NLP, embeddings, transformers |
| Generative and reliable models | 26–32 | Autoencoders, GANs, evaluation, regularization, tuning, persistence, deployment |
| Practice | 33 | End-to-end projects |

## Chapter index

1. Python for Deep Learning
2. NumPy
3. Pandas
4. Matplotlib and Seaborn
5. Tensor Basics
6. Neural Network Fundamentals
7. Perceptron
8. Activation Functions
9. Loss Functions
10. Optimizers
11. Backpropagation
12. Gradient Descent
13. Artificial Neural Networks
14. TensorFlow Basics
15. Keras Basics
16. PyTorch Basics
17. Image Data Preprocessing
18. Convolutional Neural Networks
19. Transfer Learning
20. Data Augmentation
21. Recurrent Neural Networks
22. LSTM and GRU
23. Natural Language Processing Basics
24. Word Embeddings
25. Transformers Basics
26. Autoencoders
27. Generative Adversarial Networks
28. Model Evaluation
29. Regularization and Dropout
30. Hyperparameter Tuning
31. Model Saving and Loading
32. Deployment Basics
33. End-to-End Deep Learning Projects

## The most important mental model

A neural network receives numbers, performs a sequence of mathematical operations, produces a prediction, measures how wrong that prediction is using a **loss function**, and adjusts its trainable **parameters** to reduce that loss.

- **Tensor:** a multi-dimensional container of numbers.
- **Parameter:** a value learned during training, usually a weight or bias.
- **Activation:** the output of a neuron after applying an activation function.
- **Forward pass:** moving input data through the network to produce a prediction.
- **Loss:** a number measuring prediction error.
- **Gradient:** information about how changing a parameter changes the loss.
- **Backpropagation:** an efficient method for calculating gradients through network layers.
- **Optimizer:** the algorithm that uses gradients to update parameters.
- **Epoch:** one complete pass through the training dataset.
- **Batch:** the subset of examples processed together in one training step.
- **Inference:** using a trained model to produce predictions.

## How to study

1. Read the intuition before the equations.
2. Trace tensor shapes through every operation. Shape mismatches are one of the most common deep-learning errors.
3. Run code cells in order and compare outputs with the text.
4. For training notebooks, inspect loss and metrics across epochs rather than looking only at the final score.
5. Change one parameter at a time and predict what will happen.
6. Complete the practice exercises before moving to the next topic.

## Environment setup

Create an isolated environment and install the repository dependencies:

```bash
python -m venv .venv
# Windows PowerShell:
.venv\Scripts\Activate.ps1
# macOS / Linux:
source .venv/bin/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
jupyter notebook
```

Deep-learning framework installation can depend on operating system, Python version, GPU and CUDA support. If TensorFlow or PyTorch fails to install, use the official installation selector rather than guessing a CUDA package.

- [TensorFlow installation](https://www.tensorflow.org/install)
- [PyTorch installation selector](https://pytorch.org/get-started/locally/)

## Projects

The project folder includes image classification, object detection, sentiment analysis, text classification, face-mask detection, handwritten-digit recognition, chatbot, time-series forecasting, medical-image classification and recommendation-system exercises. Some projects use tiny educational data files; these demonstrate workflow and should not be mistaken for production-grade datasets or validated medical systems.

## Further reading

- [Deep Learning book](https://www.deeplearningbook.org/)
- [Dive into Deep Learning](https://d2l.ai/)
- [TensorFlow tutorials](https://www.tensorflow.org/tutorials)
- [PyTorch tutorials](https://pytorch.org/tutorials/)
- [GeeksforGeeks Deep Learning](https://www.geeksforgeeks.org/deep-learning/)
- [Papers with Code](https://paperswithcode.com/)

## Study tracker

Open `study-tracker.html` in a browser to track chapter completion.
