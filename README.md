Ex.No.6 Development of Python Code Compatible with Multiple AI Tools

Aim: 

Write and implement Python code that integrates with multiple AI tools to automate the task of interacting with APIs, comparing outputs, and generating actionable insights with Multiple AI Tools.

Explanation:

Develop a python code that integrates multiple AI tool by interacting with their APIs.
Compare outputs from different APIs.
Analyze the response and the Output.

The aim is to understand how to request help from AI tools for tasks like writing Python code, integrating with APIs, comparing outputs, and generating actionable insights.
# program:
'''
# POSITIVE ANALYSIS

from nltk.sentiment import SentimentIntensityAnalyzer
import nltk

# Download VADER lexicon
nltk.download('vader_lexicon')

# Simulated AI-generated text
generated_text = """
This smartphone offers outstanding battery life and an intelligent AI camera 
that captures stunning photos.
"""

print("Generated Review:\n")
print(generated_text)

# Sentiment analysis
sia = SentimentIntensityAnalyzer()
sentiment = sia.polarity_scores(generated_text)

print("\nSentiment Analysis:")
print(sentiment)

# Insight generation
if sentiment['compound'] > 0:
    print("\nInsight: The review is positive and suitable for marketing promotion.")
else:
    print("\nInsight: The review tone is neutral or negative.")

# NEGATIVE ANALYSIS

from nltk.sentiment import SentimentIntensityAnalyzer
import nltk

# Download VADER lexicon
nltk.download('vader_lexicon')

# Simulated negative review text
negative_text = """
This smartphone has very poor battery life and the camera quality is disappointing.
"""

print("\nNegative Review:\n")
print(negative_text)

# Sentiment analysis
sia = SentimentIntensityAnalyzer()
negative_sentiment = sia.polarity_scores(negative_text)

print("\nNegative Sentiment Analysis:")
print(negative_sentiment)

# Insight generation
if negative_sentiment['compound'] < 0:
    print("\nInsight: The review is negative and may require product improvement.")
else:
    print("\nInsight: The review tone is neutral or positive.")
'''

Result: 
<img width="1616" height="455" alt="Screenshot 2026-06-03 235853" src="https://github.com/user-attachments/assets/9ecda813-a411-4aef-b31f-9fab405d8a30" />
<img width="1920" height="393" alt="Screenshot 2026-06-03 235951" src="https://github.com/user-attachments/assets/0bd62eb4-df54-4fe8-9439-6245b2fb21e8" />
