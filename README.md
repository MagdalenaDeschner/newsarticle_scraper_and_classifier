## 1) Web scraping
- file `scraper.py`
- scrape german news articles and their category label from www.n-tv.de 
- used packages:
    - `urllib.request` to get http pages
    - `BeautifulSoup` to parse html

## 2) Cleaning and vectorization of text
- file `preprocessing.py`
- split data into train and test set
- fit tfidf vectorizer on train data
- vectorize train data with fitted tfidf  
- used packages:
    - `sklearn.feature_extraction.text` to vectorize text with tfidf
    - `sklearn.model_selection` to split data into train and test

## 3) Text classification
- file `classifier.py`
- train [GaussianNB](http://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.GaussianNB.html#sklearn.naive_bayes.GaussianNB) classifier on articles' body and category label 
- used packages:
    - `sklearn.naive_bayes` to implement GaussianNaiveBayes classifier

## 4) Prediction
- file `predict.py`
- transform test data with fitted tfidf vectorizer
- predict category label for test data
- get classification report and confusion matrix to evaluate results
- used packages:
  - `sklearn.metrics` for model evaluation capabilities

<br>
<br>

### *Next steps*:
- define classes and methods for articles to optimize work flow
- develop Flask API for prediction