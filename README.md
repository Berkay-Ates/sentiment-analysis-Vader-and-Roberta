# Sentiment Analysis in Python

This Python notebook demonstrates sentiment analysis using two different techniques: VADER (Valence Aware Dictionary and Sentiment Reasoner) with a Bag of Words approach and the Roberta Pretrained Model from HuggingFace.

## Step 0: Read in Data and NLTK Basics
Install necessary libraries and load the dataset. Perform a quick exploratory data analysis (EDA) and tokenize an example sentence.

## Step 1: VADER Sentiment Scoring
Utilize the NLTK library's SentimentIntensityAnalyzer to obtain negative, neutral, and positive scores for the text. This approach involves removing stop words, scoring each word, and combining scores to calculate a total score. Visualize the sentiment scores and explore if comments with a 5-star rating are more positive than others.

## Step 2: Roberta Pretrained Model
Use a pre-trained model, specifically the "cardiffnlp/twitter-roberta-base-sentiment" model from HuggingFace. Tokenize the example sentence and obtain sentiment scores using the Roberta model. Apply this process to the entire dataset.

## Step 3: Combine and Compare
Combine the results from both VADER and the Roberta model and compare them. Visualize the results using pair plots.

## Step 4: Review Examples
Review examples where the model scores and review scores differ the most, specifically focusing on positive 1-star and negative 5-star reviews.

## Extra: The Transformers Pipeline
Demonstrate a quick and easy way to run sentiment predictions using the Transformers library's pipeline.

**Note:** Make sure to install the required libraries before running the code:
```bash
pip install seaborn tqdm transformers
