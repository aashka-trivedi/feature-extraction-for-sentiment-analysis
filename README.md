# feature-extraction-for-sentiment-analysis
Exploring the different Feature Extraction methods for Twitter Sentiment Analysis.

During Sentiment Analysis, we try to lable the tweets according to its sentiment- here, a tweet having lable '1' means it has negative connotations, and '0' refers to neutrality. We use the [Kaggle Text Analysis dataset](https://www.kaggle.com/chiranjeevbit/text-analysis) for sentiment analysis.

The main goal here is to explore the different ways of feature extraction, not optimising the model as a whole. Feature extraction is done by the following methods:

1. [Bag Of Words Features](https://machinelearningmastery.com/gentle-introduction-bag-words-model/): creates a matrix of the unique tokens (in all documents in a corpus) and their respective frequencies. This will not see the context of the words, merely the presence of the word.

2. [TF-IDF Features](https://medium.com/acing-ai/what-is-tf-idf-in-feature-engineering-7f1ba81982bd): like BOW, but gives more weight to rare words. That is, words that occur frequently in only a few tweets are given more importance than words that occur in all tweets.

3. Word Embeddings ([Word2Vec](https://medium.com/@eiki1212/feature-extraction-in-natural-language-processing-with-python-59c7cdcaf064)): these are representations of texts that preserve the semantics (in a way). Here, words with similar meaning will be mapped to a similar representation. Word2Vec gives a numerical representation of a word,that preserve the relationship between words (such as synonyms or antonyms). 
