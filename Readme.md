# Search Engine 🔎📚:

## Part 1: 

**File:** *Inverted Index.ipynb*

Using the dataset provided :

a) Develop an inverted index - dictionary and postings list using standard data
structures in Python (Dictionary, Json Formats, List...). You can choose to tokenize
and stem / lemmatize the data. Use NLTK 3 libraries
(http://www.nltk.org/install.html) (NLTK Book -- http://www.nltk.org/book).
Develop TF-IDF scoring for queries. Run on the query set given. Tabulate the speed
of execution. Calculate precision, recall and MAP for the given query set for top 10
results.

b) Build an inverted index using python based Elasticsearch -
https://pypi.python.org/pypi/elasticsearch. Now again tabulate the speed as well as
Precision/Recall/MAP for top 10 and compare with the previous approach.
Output expected for submission: Code + document with tabulations of speed,
precision/recall/MAP, and comparison between the two approaches.

## Part 2: 

**File:** *Inverted Index.ipynb*

Use the index and model of part 1-a. Apply pseudo relevance feedback assuming
top 5 documents to be relevant. In the query updation equation for pseudo relevance
feedback, assume beta=1-alpha. Vary alpha with a step of 0.1 between [0,1], and for each
alpha value, perform the pseudo relevance feedback. Report the alpha which maximizes the
MAP. Does this improve the performance of the IR engine? Also, submit the code.

## Part 3: 

**File:** *Document Ranking.ipynb*

Using the same dataset now to show the comparative behaviors of three different
document ranking models - 

a) TF-IDF 

b) Binary Independence Model and 

c) Language Model. 

For each case, mention the model you are using and corresponding assumptions.
Use precision/Recall/MAP for performance measurements and tabulate the speed of
execution for each model. Submit the code along with a document containing the
comparison results.


## Part 4: 

**File:** *Classifier.ipynb*

Assume the documents relevant to each query belong to a separate class. If there
are one or more documents which are relevant to more than one query, ignore them. These
classes work as ground truth classes. From each class of documents, choose 70% randomly
for training and leave the remaining 30% as test data. Apply Rocchio classifier and KNN
classifier with K=1, 3 and 5 on these test documents and report the Precision, Recall, F1
score and accuracy for each of these three classifiers. Submit the code and results.
