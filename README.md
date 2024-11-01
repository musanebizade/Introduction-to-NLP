# NLP in TensorFlow

This repository contains a Jupyter notebook implementing Natural Language Processing (NLP) using TensorFlow and TensorFlow Hub, focusing on text classification with transfer learning. The project leverages the Universal Sentence Encoder (USE) for encoding text into embeddings and builds a classification model to demonstrate transfer learning in NLP.

## Contents

- **NLP_in_Tensorflow.ipynb**: The main notebook file containing the code for text preprocessing, model creation, and training.
- **Universal Sentence Encoder (USE)**: The model uses a pre-trained Universal Sentence Encoder from TensorFlow Hub for generating text embeddings.

## Features

- **Transfer Learning with Universal Sentence Encoder (USE)**: The notebook uses a pre-trained USE layer to embed input text, allowing it to learn from pre-trained embeddings without extensive labeled data.
- **Custom Keras Layer Integration**: Includes a custom Keras layer for compatibility with TensorFlow's functional API.
- **Binary Text Classification**: The model is designed to perform binary classification on text data, which can be adapted to other NLP tasks by modifying the architecture or dataset.
- **Model Evaluation and Visualization**: The notebook provides steps for model evaluation, including accuracy metrics and loss/accuracy visualizations.

## Requirements

To run this project, you will need:

- Python 3.6+
- TensorFlow 2.x
- TensorFlow Hub
- Jupyter Notebook or JupyterLab (if running locally)

## Model Overview

The model structure is as follows:

- **Input Layer**: Receives input text in string format.
- **Universal Sentence Encoder Layer**: Embeds the text into a high-dimensional vector.
- **Dense Layers**: Adds fully connected layers for classification.
- **Output Layer**: Outputs a probability for binary classification.

## Notes

- **Data Preprocessing**: Ensure that your text data is preprocessed to match the expected input format.
- **Fine-tuning**: The Universal Sentence Encoder is frozen in this example, but you can set `trainable=True` to fine-tune it on your dataset if desired.

## Troubleshooting

- **Keras Layer Compatibility**: The notebook includes a custom wrapper for the Universal Sentence Encoder to resolve compatibility issues with Keras and TensorFlow functions.
