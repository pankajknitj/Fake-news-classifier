# Fake-news-classifier
Classifier able to detect fake news of any country news ,language must be english.
## Data source
https://www.kaggle.com/c/fake-news/data
## kaggle notebook link
https://www.kaggle.com/kagglepankaj/fake-news-classifier-with-lightgbm-90-accuracy
## Preprocessing steps
1.remove all Non alphabetic char and punctuations.
2.convert to lower case.
3.Lemmatize the word(converting to root form).
## Feature generation
1.Count the number of noun,proper noun,pronouns by pos tagging(part of speech tagging).
2.Count the number of person,place,organisation,political groups in the news article.
## Vectorization (bags of word).
Created vector using n-grame(10) Tfidf vectorizer, combined this with the previously created features.
## feature selection.
As the number of features is huge we cann't go for simple feature selection, so i choosed dimensionality reduction by **NMF** (Non negative matrix factorization)
## Model building.
Finally i trained a Light gbm model and got accuracy of 90%.

