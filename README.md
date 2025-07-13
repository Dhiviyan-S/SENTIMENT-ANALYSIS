# Import the library
from textblob import TextBlob

# Input text
text = input("Enter a sentence for sentiment analysis: ")

# Create TextBlob object
blob = TextBlob(text)

# Get sentiment polarity
polarity = blob.sentiment.polarity

# Print result
if polarity > 0:
    print("Positive Sentiment 😊")
elif polarity < 0:
    print("Negative Sentiment 😠")
else:
    print("Neutral Sentiment 😐")
