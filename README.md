# Hotel-Reviews

**Goal**
There are two goals to this initiative
1. To do a sentiment analysis of Hotel reviews and predict its classification
2. To predict the Reviewer score based on Hotel features and/or reviews

**Data**: [Dataset from Booking.com publicly available in Kaggle](https://www.kaggle.com/jiashenliu/515k-hotel-reviews-data-in-europe)

**Hotel_reviews_Sentiment_Analysis.ipynb**
nltk library and TFID Vectorization are used to generate TFID weights of words in reviews. Since the original data classifies reviews as Positive and Negative, the same is used to train and predict. Further analysis of frequency of words is done.

**Hotel_Review_Prediction.ipynb**
Regression models to predict Review Scores of hotels are generated.
- Considering the TFID values of reviews
- Considering the hotel features as well as TFID values
- Considering only the hotel features
XGB Regression is used for prediction. An error rate of nearly 30% is seen (considering +/- 1 rating is acceptable)
