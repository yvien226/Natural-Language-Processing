# Amazon Food Review Sentiment Analysis Comparison

The purpose of this notebook is to perform sentiment analysis on Amazon fine food reviews and explore different techniques to understand the pros and cons of using each technique, speed and accuracy in particular.

The techniques we explored are:
1. VADER (Valence Aware Dictionary and Sentiment Reasoner) = Machine Learning (ML)
2. RoBERTa (Robustly Optimized BERT-Pretraining Approach) = large language model (LLM)

<br>

## About Amazon Fine Food Review Dataset
Data is available in Kaggle: https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews

This dataset consists of reviews of fine foods from amazon. The data span a period of more than 10 years, including all ~500,000 reviews up to October 2012. Reviews include product and user information, ratings, and a plain text review. It also includes reviews from all other Amazon categories.

The 1-5 star rating will be used as the target and compare with the predicted sentiment from the techniques.

<br> 

## About VADER and RoBERTa
1. VADER is a rule based sentiment analyser for NLTK module in which the terms are generally labeled as per their semantic orientation as either positive or negative. It is a typical bag-of-word type model, it takes each word and scored individually and combined to the total score, hence it doesn't take relationship words into account 

2. RoBERTa is a pre-trained moddel by hugging faces. It is considered as large language model/deep learning model, having trained with massive full sentences datasets. The model not only accounts for the words, but also the context related to other words, hence it can guess the polarity of the overall idea of the author pretty well


<br>

## Script/Notebook
- [Amazon Food Reviews Sentiment Analysis with VADER and RoBERTa.ipynb](https://github.com/yvien226/Natural-Language-Processing/blob/main/Food%20Review%20Sentiment%20Analysis%Comparison/Amazon%20Food%20Reviews%20Sentiment%20analysis%20with%20VADER%20and%20RoBERTa.ipynb) : A notebook which compares the 2 different techniques using Amazon food reviews dataset.

<br>

## Steps to run the notebook
1. Download data from Kaggle and save it in `Data/` folder
2. Ensure you have installed all libraries listed below
3. Run the notebook

<br>

## Python Libraries
- pandas
- numpy
- matplotlib
- seaborn
- spacy
- nltk
- vaderSentiment
- scikit-learn
- pytorch
- tqdm
- transformers
- softmax


