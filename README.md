# NLP Representation Learning and Machine Translation

## Overview

This repository contains Natural Language Processing projects completed as part of my MSc Artificial Intelligence at Heriot-Watt University.

The work explores two connected areas of NLP:

1. Representation learning using Word2Vec embeddings
2. Neural machine translation using BiLSTM, attention, and Transformer models

The projects demonstrate experience in training, evaluating, and analysing NLP models using semantic similarity, analogy reasoning, BLEU scores, training curves, and qualitative translation analysis.

## Project 1: Word2Vec Representation Learning

This project investigated how different training settings affect the quality of learned word embeddings.

Key tasks included:

* Training Word2Vec models on different corpus sizes
* Evaluating semantic similarity using cosine similarity and Spearman correlation
* Comparing small and large corpus embeddings
* Exploring the effect of vector size, context window, and epochs
* Analysing word analogies and gender bias in pretrained embeddings

### Key Findings

* Larger training corpora produced stronger semantic representations than smaller corpora.
* The best tuned Word2Vec model achieved a Spearman correlation of approximately 0.644.
* Pretrained Google News Word2Vec embeddings achieved stronger performance, with a Spearman correlation of approximately 0.683.
* Analogy analysis showed that pretrained embeddings can encode social and gender-based stereotypes.

## Project 2: Neural Machine Translation

This project explored neural machine translation using deep learning sequence models.

Key tasks included:

* Implementing BiLSTM encoder-decoder models
* Applying attention mechanisms
* Comparing model capacity and training behaviour
* Evaluating translation quality using BLEU scores
* Analysing generated translations and model errors
* Exploring Transformer-based translation models

### Key Findings

* Increasing model capacity improved translation performance substantially.
* Medium-sized models achieved stronger BLEU scores than smaller models.
* The best medium BiLSTM model achieved a BLEU score of approximately 49.17.
* Training larger models was limited by available computational resources.
* BLEU scores provided useful quantitative comparison, but qualitative analysis was also needed to understand translation errors.

## Technologies Used

* Python
* PyTorch
* Gensim
* NLTK
* NumPy
* pandas
* Weights & Biases
* Jupyter Notebook

## Repository Structure

```text
word2vec/
  word2vec-representation-learning.ipynb

machine-translation/
  neural-machine-translation.ipynb

images/
  project screenshots and result figures
```

## Notes

This repository is intended for portfolio and educational purposes. Datasets and large trained model files are not included.

## Author

Mercy Nthiwa
MSc Artificial Intelligence
Heriot-Watt University

