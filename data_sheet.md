# Datasheet: Sentence Complexity Predictor

### Model Details

Name: Sentence Complexity Predictor
Version: 1.0
Date: 2023-07-25
Framework: sklearn, gensim (Word2Vec)
Model Type: Supervised - Regression
Intended Use: Predicting the complexity of English sentences in children's literature.

### Data Collection

Data Source: 

1) NLTK : 

Download the brown corpus and the list of stopwords
nltk.download('brown')
nltk.download('stopwords')
childrens_text = brown.words(categories='lore')

2) Kaggle: https://www.kaggle.com/datasets/edenbd/children-stories-text-corpus

The data used to train and evaluate the model comes from two corpora: the Brown Corpus and a new corpus of children's fairy tales. The Brown Corpus is a collection of documents that are broadly representative of English texts. The fairy tales corpus consists of a collection of children's stories collected and compiled specifically for this project.

Who was involved in the data collection process? For the Brown Corpus, the data collection was performed by Henry Kučera and W. Nelson Francis at Brown University in the 1960s. The fairy tales corpus was collected and compiled by the project team.

How was the data collected? The data from the Brown Corpus was collected in the 1960s and is a broadly representative collection of English texts. The fairy tales corpus was collected from various online sources of children's literature and compiled into a single dataset for this project.

Does the dataset relate to people? The dataset does not contain personal data. It consists of English sentences from the Brown Corpus and the fairy tales corpus.

### Data Preprocessing

What preprocessing/cleaning was done? The sentences from both corpora were tokenized, and each word was lowercased. The sentences were then split into a training set and a test set.
Was the “raw” data saved in addition to the preprocessed/cleaned data? (Yes/No) Yes, the raw data was saved. It can be reprocessed or cleaned differently if necessary.

### Data Distribution

How was the data split between training and testing? The data was split into a training set and a test set using a 80-20 split. The split was performed using scikit-learn's train_test_split function with a random seed to ensure reproducibility.

### Data Maintenance

Is there a plan to update the dataset? (Yes/No) No, there is no current plan to update the dataset. The model can be retrained with new data if necessary.

