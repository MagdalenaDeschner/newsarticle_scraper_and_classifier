## 1) Web scraping
- file `scraper.py`
- Scrape german news articles and their category label from www.n-tv.de 
- used packages:
    - `urllib.request` to get http pages
    - `BeautifulSoup` to parse html

## 2) Cleaning and vectorization of text
- file `preprocessing.py`
- clean articles
- use tfidf to vectorize articles into words 
- used packages:
    - `sklearn.feature_extraction.text` to vectorize text with tfidf
    - `sklearn.model_selection` to split data into train and test

## 3) Text classification
- file `classifier.py`
- Train classifier on articles' body and category label to automatically classify future news

## 4) Prediction
- file `predict.py`

### *Next steps*:
- optimize ML model:
    - try out different classifiers
    - try out different text representation
- define classes and methods for articles to optimize work flow