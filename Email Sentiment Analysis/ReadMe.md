# Email Sentiment Analysis

The original intention of this project is to perform sentiment analysis on my work emails to understand if the message I received or the sender are generally positive, negative or neutral. Sentiment analysis uses natural language processing to recognise the emotional tone behind words. 

The Enron email analysis uses the same method as above to process and analyse the data with the Enron email dataset. It was obtained by the Federal Energy Regulatory Commission during the investigation of Enron Corporation's collapse. The dataset is available to the [public](https://www.cs.cmu.edu/~./enron/).

## Script/Notebook
- [Read emails and basic sentiment analysis.py](https://github.com/yvien226/Natural-Language-Processing/blob/main/Email%20Sentiment%20Analysis/Read%20emails%20and%20basic%20sentiment%20analysis.py) : General code for reading outlook emails and sentiment analysis.
- [Enron 1000 email analysis.ipynb](https://github.com/yvien226/Natural-Language-Processing/blob/main/Email%20Sentiment%20Analysis/Enron%201000%20email%20analysis.ipynb) : A notebook which extracts the first 1000 Enron emails and its analysis.

## Steps
1. Download email inbox data from outlook and save into csv file
2. Read emails and perform data preprocessing, this includes:
    - Remove smtp mails
    - Remove signatures
    - Identify sender and receiver
3. Text Processing: Using Spacy to process the body of the email:
    - Remove entities (city names, person's name, geographical places)
    - Remove stopwords (I, is, you, we, for, and etc)
    - Remove punctuation (!,.-?#:)
    - Remove spaces
    - Lemmatisation (Grouping similar words into single word
4. Perform sentiment analysis on each word using [VADER (Valence Aware Dictionary for Sentiment Reasoning)](https://github.com/cjhutto/vaderSentiment) and count the number of positive, neutral and negative words in each email content.
5. Save results into csv/excel file and visualise the data.

## Data Visualisation
Click [here](https://app.powerbi.com/view?r=eyJrIjoiOTgyZmM4OTctZDQ5NS00M2VjLWEyMjEtNGU1ZDI3MjkwNDkyIiwidCI6ImY5OGI0MDAzLTIzY2UtNGQyNS1iZmM2LWU0Nzg1YzNlMGUyZiJ9) to view the data visualisation for Enron's first 1000 Email analysis 

## Python Libraries
- pandas
- spacy
- nltk
- vaderSentiment


