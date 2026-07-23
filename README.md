# Deep Learning Learning Path

This repository is organized as a beginner-friendly deep learning study library. Each numbered folder focuses on one topic and contains a self-contained notebook with explanations, runnable code, visual examples where useful, and practice exercises.

## Learning Path

Start with Python, NumPy, Pandas, and visualization. Then move into tensors, neural network fundamentals, optimization, and backpropagation. After that, study practical frameworks such as TensorFlow, Keras, and PyTorch. The later folders introduce computer vision, NLP, transformers, generative models, evaluation, regularization, tuning, saving, deployment, and end-to-end projects.

## Folder List

- `01. Python For Deep Learning`
- `02. NumPy`
- `03. Pandas`
- `04. Matplotlib And Seaborn`
- `05. Tensor Basics`
- `06. Neural Network Fundamentals`
- `07. Perceptron`
- `08. Activation Functions`
- `09. Loss Functions`
- `10. Optimizers`
- `11. Backpropagation`
- `12. Gradient Descent`
- `13. Artificial Neural Networks`
- `14. TensorFlow Basics`
- `15. Keras Basics`
- `16. PyTorch Basics`
- `17. Image Data Preprocessing`
- `18. Convolutional Neural Networks`
- `19. Transfer Learning`
- `20. Data Augmentation`
- `21. Recurrent Neural Networks`
- `22. LSTM And GRU`
- `23. Natural Language Processing Basics`
- `24. Word Embeddings`
- `25. Transformers Basics`
- `26. Autoencoders`
- `27. Generative Adversarial Networks`
- `28. Model Evaluation`
- `29. Regularization And Dropout`
- `30. Hyperparameter Tuning`
- `31. Model Saving And Loading`
- `32. Deployment Basics`
- `33. End-To-End Deep Learning Projects`

## End-To-End Projects

- `01. Image Classification`
- `02. Object Detection`
- `03. Sentiment Analysis`
- `04. Text Classification`
- `05. Face Mask Detection`
- `06. Handwritten Digit Recognition`
- `07. Chatbot`
- `08. Time Series Forecasting`
- `09. Medical Image Classification`
- `10. Recommendation System`

## Recommended Study Order

1. Complete folders `01` to `04` for Python data skills.
2. Complete folders `05` to `12` for the math and training loop intuition.
3. Complete folders `13` to `16` for practical model-building frameworks.
4. Complete folders `17` to `25` for images, sequences, NLP, and transformers.
5. Complete folders `26` to `32` for advanced model families and production basics.
6. Work through `33. End-To-End Deep Learning Projects` to practice complete workflows.

## How to Run the Notebooks

Create and activate a virtual environment, then install the dependencies:

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

Launch Jupyter:

```bash
jupyter notebook
```

Open the notebooks in numbered order. Each notebook is designed to be run from inside its own folder so relative dataset paths work correctly.

## Notes for Beginners

- Run every cell from top to bottom.
- Read the markdown before running the code.
- Change small values and re-run cells to build intuition.
- Complete the practice exercises before moving to the next topic.
- For TensorFlow and PyTorch notebooks, install the full `requirements.txt` first.
