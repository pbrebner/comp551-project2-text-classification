# Text Classifier with Scikit-Learn

Classification of Textual Data using the following machine learning models: Logistic Regression, Decision Trees, Support Vector Machines, Ada Boost, and Random Forest. The project goal is to determine whine machine learning algorithm performs the best and text classification/sentiment analysis.

writeup.pdf: The main report of the project

## Datasets
Two textual datasets were used to test the machine learning algorithms

### 20 NewsGroups Dataset
The 20 Newsgroups dataset is a collection of approximately 20,000 newsgroup documents, partitioned (nearly) evenly across 20 different newsgroups.

Supervised learning algorithms will require a category label for each document in the training set. In this case the category is the name of the newsgroup which also happens to be the name of the folder holding the individual documents.

### IMDB_Reviews Dataset
The IMDB Review dataset contains movie reviews along with associated binary sentiment polarity labels.The main dataset contains 50,000 reviews split evenly between a train and test set (25,000 each). The distribution of positive and negative labels are balanced.

In the entire dataset, no more than 30 movie reviews are allowed for the same movie. This is because reviews for the same movie tend to have correlation. Further, the train and test sets contain a disjoint set of movies, so no significant performance is obtained by memorizing movie-unique terms and their associated with observed labels.

For the train/test set a negative review has a score <= 4 out of 10 and a positive review has a score >= 7 out of 10. Reviews with a more neutral score were not included in the dataset.

## Jupyter Notebook Files:
1. NewsGroup Dataset.ipynb : Loading, Text Preprocessing, and Multi-Class Classification of the 20 NewsGroup Dataset
2. IMDB_Reviews_Dataset_tfidf: Loading, tect Preprocessing (Unigram with no text normalization) and Classification of the IMDB Dataset
3. IMDB_Reviews_Dataset_tfidf_stemming: Loading, Text Preprocessing (Unigram with Stemming) and Classifcation of IMDB Dataset
4. IMDB_Reviews_Dataset_tfidf_lemming: Loading, Text Preprocessing (Unigram with Lemmatization) and Classifcation of IMDB Dataset
5. IMDB_Reviews_Dataset_tfidf_bigram: Loading, text Preprocessing (Bigram with no text normalization) and Classifcation of IMDB Dataset
    
Each Jupyter Notebook file will download/load the respective dataset and run through the required text preprocessing and classifcation models. The IMDB Dataset jupyter notebook files are all the same except for the preprocessing technique used before classification. The IMDB_Reviews_Dataset_tfidf uses the same preprocessing techniques as the NewsGroup Dataset jupyter notebook file.

<object data="writeup.pdf" type="application/pdf" width="700px" height="700px">
    <embed src="writeup.pdf">
        <p>Please read writeup.pdf for full results and discussion. You can download the PDF to view it: <a href="writeup.pdf">Download PDF</a>.</p>
    </embed>
</object>
