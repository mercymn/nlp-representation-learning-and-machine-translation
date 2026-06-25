# NLP Representation Learning and Machine Translation

## Overview

This repository contains Natural Language Processing projects completed during my MSc Artificial Intelligence at Heriot-Watt University.

The work investigates two connected areas of NLP:

1. Representation learning using Word2Vec embeddings
2. Neural machine translation using BiLSTM, attention, and Transformer models

The projects evaluate how modelling choices influence representation quality and translation performance through systematic experimentation and quantitative evaluation.

# Project 1 – Word2Vec Representation Learning

## Objective

Investigate how corpus size and model hyperparameters influence the quality of learned semantic word representations.

## Methodology

The project trained Word2Vec embeddings on small and large WikiText corpora and evaluated representation quality using cosine similarity, Spearman correlation against human similarity judgements, pretrained Google News embeddings, analogy reasoning, and hyperparameter comparisons.

### Key Findings

- Larger corpora produced substantially stronger semantic representations than smaller datasets.
- Increasing embedding dimensionality improved performance on the large corpus, but provided limited benefit for the small corpus.
- The best tuned Word2Vec model achieved a Spearman correlation of approximately 0.644.
- Pretrained Google News embeddings achieved stronger alignment with human semantic judgements, with a Spearman correlation of approximately 0.683.
- Analogy experiments demonstrated that learned embeddings captured semantic relationships while also revealing gender-related biases inherited from training data.

## Limitations

The custom embeddings were trained on relatively small corpora compared with industrial-scale pretrained models. Consequently, evaluation scores remained below the Google News embeddings despite hyperparameter optimisation. Future work could investigate larger corpora, subword embeddings such as FastText, or contextual language models.

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

