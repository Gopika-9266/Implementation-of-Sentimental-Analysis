# Implementation-of-Sentimental-Analysis

The process of sentiment analysis using VADER model can be described as follows:

## Read the input text:
The first step is to read the input text. This can be done using a variety of methods, such as reading a file, receiving input from a user, or scraping text from a website.

## Clean the text:
Once the text has been read,it is important to clean it.This involves removing any punctuation,stop words or other noise that could interfere with the sentiment analysis process.

## Calculate the sentiment scores:
The next step is to calculate the sentiment scores for the text. This is done by using a sentiment analysis model, such as VADER.

## Interpret the results:
The final step is to interpret the results of the sentiment analysis. This involves understanding the meaning of the sentiment scores and how they relate to the text. VADER is a lexicon- and rule-based sentiment analysis tool that is specifically designed to work with social media text. It is a free and open-source tool that can be used to analyze text in a variety of languages. VADER is a popular choice for sentiment analysis because it is easy to use and produces accurate results.

## Program:
```
Developed By: Gopika R
Reg No: 212222240031
```
```
import nltk
from nltk.sentiment import SentimentIntensityAnalyzer

nltk.download('vader_lexicon')

sia = SentimentIntensityAnalyzer()

text = input("Enter a sentence to analyze: ")

scores = sia.polarity_scores(text)

print("Positive score:", scores['pos'])
print("Negative score:", scores['neg'])
print("Neutral score:", scores['neu'])
print("Compound score:", scores['compound'])
```

## Output:

![Screenshot 2023-11-10 092035](https://github.com/Gopika-9266/Implementation-of-Sentimental-Analysis/assets/122762773/0e2506f0-b441-4ef5-9b29-e5ddd8200ac8)



