Sequence-to-Sequence Models for Tamil Transliteration
This repository contains implementation and experimentation with sequence-to-sequence (seq2seq) models for Tamil transliteration, with a focus on comparing models with and without attention mechanisms. The project utilizes the Dakshina dataset, which contains parallel data of words in Latin script and their equivalent in Tamil script.

WandB Report - https://wandb.ai/surendarmohan283-indian-institute-of-technology-madras/DA6401_A3/reports/Surendar-s-Assignment-3--VmlldzoxMjgxOTE4Mg

## Repository Structure
## 1. a3-with-attention.ipynb
- This notebook implements a sequence-to-sequence model with attention mechanism. Key components include:

- Data download and preprocessing for the Dakshina Tamil dataset
  Implementation of encoder-decoder architecture with attention
  Character-level vocabulary handling
  Training and evaluation pipelines
  Hyperparameter tuning using Weights & Biases
  Various model configurations (LSTM, GRU, RNN) with different hyperparameters

- The attention mechanism implemented is a form of Bahdanau attention, which allows the decoder to focus on different parts of the input sequence when generating each output character.
## 2. a3-without-attention.ipynb
- Similar to the first notebook, but implements a sequence-to-sequence model without attention for comparison. This serves as a baseline to understand the benefits of attention mechanisms in transliteration tasks.
- Key components:

  Similar architecture to the attention model but without the attention mechanism
  Same data processing pipeline and evaluation metrics
  Comparable hyperparameter searching strategy

## 3. vis-att.ipynb
- This notebook focuses on visualizing the attention mechanisms to provide insights into how the model works:

- Implementation for loading trained models
  Visualization code for attention weights
  Analysis of attention patterns across different examples
  Interpretation of how the model learns the mapping between Latin and Tamil scripts

Requirements
The project requires:

Python 3.x
PyTorch
NumPy
Pandas
Matplotlib
Weights & Biases
