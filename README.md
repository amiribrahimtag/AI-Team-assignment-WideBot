# AI-Team-assignment-WideBot

__Training process__

1. Importing Libraries

2. Loading Data

3. Data Exploration

4. Data Preprocessing
* Created a regular expression pattern that matches any non-Arabic letter then replaced any non-Arabic letters in the "text" column with an empty string
* Removed Arabic punctuation
* Replaced any 2 or more spaces with 1 space
* Defined function to normalize arabic text
* Defined function to remove arabic stop words
* Defined function to normalize specific letters
* Encoded the target feature

5. Exploratory Data Analysis
* Provided insights for Task 2
[ number of examples per class, top frequent n-grams generally and per class, lengths of examples in words and letters ] 
  
7. Modeling

* Splitted the data into 80/20
* Used TfidfVectorizer to convert the text data into numerical features that can be used as input to a machine learning model for classification.
* Used LinearSVC un-tuned once and with GridSearchCV once and picked the better once to interpret it's results

8. Final Results

* __art-et-culture > Class 1:__ Precision=0.86, Recall=0.87, F1-score=0.86
* __economie > Class 2:__ Precision=0.85, Recall=0.93, F1-score=0.89
* __faits-divers > Class 3:__ Precision=0.95, Recall=0.92, F1-score=0.94
* __marocains-du-monde > Class 4:__ Precision=0.89, Recall=0.87, F1-score=0.88
* __medias > Class 5:__ Precision=0.96, Recall=0.92, F1-score=0.94
* __orbites > Class 6:__ Precision=0.67, Recall=0.66, F1-score=0.67
* __politique > Class 7:__ Precision=0.76, Recall=0.80, F1-score=0.78
* __regions > Class 8:__ Precision=0.82, Recall=0.85, F1-score=0.83
* __societe > Class 9:__ Precision=0.81, Recall=0.72, F1-score=0.76
* __sport > Class 10:__ Precision=0.99, Recall=1.00, F1-score=0.99
* __tamazight > Class 11:__ Precision=0.96, Recall=0.96, F1-score=0.96


__Accuracy:__ The overall accuracy of the classifier is 0.86, which means that 86% of the samples in the test set were correctly classified.

__Precision:__ A precision of 0.86 for class 1 means that 86% of the samples predicted as class 1 were correctly classified as class 1. The precision is high (above 0.8) for most classes, indicating that the classifier has relatively few false positives.

__Recall:__ A recall of 0.87 for class 1 means that 87% of the actual samples of class 1 were correctly classified as class 1. The recall is high (above 0.8) for most classes, indicating that the classifier has relatively few false negatives.

__F1-score:__ The F1-score is high (above 0.8) for most classes, indicating that the classifier has good overall performance.


__Overall, the classifier performs well on most classes, with high precision, recall, and F1-score. Some classes (e.g. 6 and 9) have lower precision and recall, indicating that the classifier has more difficulty distinguishing between these classes. The overall accuracy of 0.86 is also relatively high, indicating that the classifier is able to classify most samples correctly.__


### Possible enhancements that could improve the performance of the classifier:

__1. Performing more in-depth analysis of misclassified instances can potentially improve the classifier's accuracy and generalization ability.__

__2. Asking Domain Experts for An Custom Stopword List.__

__3.Trying different text preprocessing techniques, such as stemming or lemmatization.__

__4.Using more advanced vectorization techniques, such as word embeddings or character-level embeddings.__

__5.Data augmentation: The current classifier uses only the available labeled data for training and evaluation. However, it may be possible to generate additional labeled data through techniques such as data synthesis or data annotation, which could improve the performance of the classifier.__

__6.Ensemble methods: The current classifier uses a single model to make predictions. However, it may be possible to improve performance by combining the predictions of multiple models using ensemble methods such as bagging or boosting.__

