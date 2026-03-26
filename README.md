# Quora-Duplication-Detection

This project aims to detect duplicate questions on Quora by utilizing Natural Language Processing (NLP) techniques, machine learning, and deep learning models. The dataset includes pairs of questions with labels indicating whether the questions are duplicates or not.

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [How to Run](#how-to-run)
- [Technologies Used](#technologies-used)
- [Future Work](#future-work)

## Overview
The project involves processing question pairs, performing text preprocessing, and extracting features to train machine learning and deep learning models for identifying duplicate questions. The models implemented in this project include:
- **Random Forest Classifier** with custom features and Word2Vec embeddings.
- **LSTM Neural Network** to further enhance accuracy using tokenized sequences and embedding layers.

## Installation

1. Clone the repository:
   ```bash
   git clone <https://github.com/aarushipateldpsv-dotcom/Quora-Duplication-Detection.git>
   cd <Quora_Duplicate_Detection>
   ```

## Dataset
The dataset contains pairs of questions from Quora with labels indicating whether they are duplicates (1) or not (0). This can be found on Kaggle or other sources, and it should be placed in the data/ folder as questions.csv.

## Methodology
### 1. Text Preprocessing
Performed tokenization, stop word removal, and stemming using NLTK to clean the question texts.
### 2. Feature Extraction
Word2Vec: Used to generate word embeddings for the questions.
Custom Features: Extracted features like word length, sentence metrics, FOG index, and sentiment analysis using TextBlob.
### 3. Machine Learning Model - Random Forest
Word embeddings were combined with custom features to train a Random Forest Classifier.
Achieved an accuracy of 83.8% on the test set.
### 4. Deep Learning Model - LSTM
Used tokenized question sequences with an embedding layer and trained an LSTM model to improve accuracy.
Achieved an accuracy of 94% using the LSTM network.

## Results
### Random Forest Accuracy: 83.8%
### LSTM Neural Network Accuracy: 94%

## How to Run
1. Open the Jupyter notebook (notebooks/quora_similarity_detection.ipynb) in a Jupyter environment:
2. Run the cells to preprocess the data, train the models, and evaluate performance.
3. For inference, you can use the inference functions to test custom question pairs.

## Technologies Used
+ Languages: Python
+ Libraries: Pandas, Numpy, Gensim, NLTK, Scikit-learn, TensorFlow, Keras
+ Techniques: Word2Vec, Text Preprocessing, LSTM, Random Forest

## Future Work
+ Experiment with more advanced NLP techniques like BERT or Transformer models.
+ Optimize the LSTM model using hyperparameter tuning.
+ Explore additional features such as POS tagging or syntactic analysis.

### THANKS FOR GIVING IT A READ!🙌 
