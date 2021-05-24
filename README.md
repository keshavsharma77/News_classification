# News_classification
BBN news Classification by Headlines using ML algorithms and perform hyperparameter tuning to improve its performance.

Text Classification is a difficult activity as it requires pre-processing steps to covert the textual data into structured form from the un-structured form. There are different steps involved in news classification. News classification process involves following main steps for classification of news article. These steps are data collection, pre-processing, feature selection, classification techniques application, and evaluating performance measures.

Objectives:
    •	To automatically classify the News text documents into one or more defined categories. 
    •	To compare different algorithms based on its Accuracy.
    •	To perform Hyperparameter Tuning to improve Accuracy.

# Concepts Used:
# 1)	Naive Bayes:
Naive Bayes is a probabilistic classifier based on text features. It calculates class labels and probability of classes. Naive bayes isn’t made up of a single algorithm for classification but it includes a large number of algorithms that work on a single principal for training classifiers and the principal states that the value of a particular feature is autonomous of value of any other feature specified in a class. In the past classification of news article naive bayes were used. But due to its incorrect parameter assessment revamped accuracy was reported. The best thing about Naive bayes algorithm is that it works equally well on both textual as well as numeric data and it is easy to implement and calculate. But it shows poor performance when the features are correlated like short text classification.
                  
Multinomial Naive Bayes is used in this project as it is used mainly for text classification. This is because it works well for data which can easily be turned into counts, such as word counts in text.

# 2)	Support Vector Machines:
SVM has been used a lot for news text classification. SVM has a unique feature that it includes both negative and positive training sets which is generally not preferred by other algorithms. Linear Support Vector Classification is used in this project. The objective of a Linear SVC (Support Vector Classifier) is to fit to the data provided, returning a "best fit" hyperplane that divides, or categorizes, the data.

# 3)	Random Forests:
Random forest, like its name implies, consists of a large number of individual decision trees that operate as an ensemble. Random Forests (RF) is an ensemble learning method for classification and regression. It uses bagging and feature randomness when building each individual tree to try to create an uncorrelated forest of trees whose prediction by committee is more accurate than that of any individual tree. We investigate the application of RF for news articles classification. Although the RF have been successfully applied to several classification problems, to the best of our knowledge they haven’t been applied to news article classification problems. An important motivation for using RF was the application of late fusion strategies based on the RF operational capabilities.

# 4)	K-nearest neighbors:
K-nearest neighbors is a simple algorithm and a non-parameterized way of classification and regression in case of pattern recognition. For using this algorithm, we need to refer K-similar text documents. It reckons the
similarity against all documents that exists in the training set and uses it for making decisions about presence of class in the desired category. Neighbor that has same class are the most probable ones for that class and the neighbors with highest probability are assigned to the specific class. K-nearest neighbors is effective and nonparameterized algorithm. The biggest pitfall is that it requires a lot of classification time and it is also difficult to find an optimal value of K. K-nearest neighbor is a type of lazy learning where function Generalization beyond the data is delayed until a query is made to the system. K-nearest neighbor is one of the simplest machine learning algorithms.
 

# 5)	TfidfVectorizer:
Word counts are a good starting point, but are very basic. One issue with simple counts is that some words like “the” will appear many times and their large counts will not be very meaningful in the encoded vectors. An alternative is to calculate word frequencies, and by far the most popular method is called TF-IDF. This is an acronym than stands for “Term Frequency – Inverse Document Frequency” which are the components of the resulting scores assigned to each word. The TfidfVectorizer will tokenize documents, learn the vocabulary and inverse document frequency weightings, and allows to encode new documents. Alternately, if it already has a learned Count Vectorizer, use it with a TfidfTransformer to just calculate the inverse document frequencies and start encoding documents.


# News Collection:
In this Project, we used a dataset from BBC News that have three columns, one has the news article Id, second having the headlines and the other contains the class it belongs to. There are 1490 rows in the data set.

# News Pre-processing:
After News collection, pre-processing is done as this information is originating from variety of sources and its cleaning is required so that it could be free from corrupted file. Information after pre-processing should be separated from random words like semicolon, double quotes, full stop, bracket, special characters and so on and also the information is converted to lower case character to get better outcomes. Information is made free from those words which show up generally in content and are known as stop words.

# Feature Selection
The feature selections in this project were done by using TF-IDF. Term Frequency-Inverse Document Frequency (TF-IDF) is a very common algorithm which is used to transform text into a meaningful representation of numbers. TF-IDF can be used for stop-words filtering in various subject fields including text summarization and classification. 

# News Headlines Classification: 
After feature selection, classification is to be done where the news headlines are classified with an aim to assign to their respective classes. The News headlines classification methods used in this Project are Naïve Bayes, Support Vector Classifier, Random Forest, Logistic Regression and KNN.

![image](https://user-images.githubusercontent.com/64605506/119396042-fa745400-bcf1-11eb-8900-38b9080c9cbc.png)

Hyper Parameter Tuning is performed on ML models to improve their Accuracies for Classification of News based on its Headlines.

After Hyper Parameter Tunning Accuracies of models increased to some extent giving better Results.
![image](https://user-images.githubusercontent.com/64605506/119396175-28599880-bcf2-11eb-83c7-8a836b06e559.png)


A successful implementation has been done to classify the News based on its Headline. In addition to it GUI using Gradio python Library is also created. Comparison between different Classification algorithm is also done. Accuracy of Models is increased using hyper parameter tuning. SVM is the best model for more Accurate classification of News.

