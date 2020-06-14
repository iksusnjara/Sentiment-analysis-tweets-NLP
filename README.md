# Sentiment-analysis-tweets-NLP
Using deep neural network to perform analysis of sentiment in tweets regarding airline companies


### Project description

Sentiment analysis, based on on Twitter data regarding its topic is non-surprisingly hot topic, given the value it can bring. Here tweets regarding airline passanger companies were collected, and labeled by human raters as positive, neutral or negative. Next, the task was to build model being able to recognize sentiment of a tweet: to automatically recognize text as being positive, negative or neutral. Further project description and dataset can be found at https://www.kaggle.com/crowdflower/twitter-airline-sentiment.

Tweet texts are first cleaned and preprocessed using NLTK Python library. It is used to remove all emoticons and other special characters and punctuation. Words are then POS tagged and reduced to their lemmata using NLTK's WordNet Lemmatizer. Finally, a number of words is choosen to be used as tokens. They are converted to vectors using embedding layer inside neural network. This layer is not pretrained, i.e. it is trained along with the model, specifically for this task. LSTM reccurent architecture is next applied on vectorized words for classification.


### Used technologies:

- Python 3.7 with JupyterLab environment
- PyTorch
- nltk
- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn
