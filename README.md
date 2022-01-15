# Youtube-Sentiment

### Objective:  
  
Youtube has removed the dislike button. The fun of disliking terrible videos like Youtube rewind are gone. Fortunately, this project can give a user insight to the sentiment of a video based on the top 50 comments. 

### Notes:  
  
Used Selenium for scraping - Beautifulsoup does not work for comments, only static pages.
Used Vader for NLP - Understands internet slang, and internet rules
  ex: 
  ` sentence = "I love pizza"
sentiment_dict = obj.polarity_scores(sentence)
print(sentiment_dict)`
`{'neg': 0.0, 'neu': 0.323, 'pos': 0.677, 'compound': 0.6369}`
`sentence = "I LOVE pizza!!"
sentiment_dict = obj.polarity_scores(sentence)
print(sentiment_dict)`
`{'neg': 0.0, 'neu': 0.266, 'pos': 0.734, 'compound': 0.7592}`
