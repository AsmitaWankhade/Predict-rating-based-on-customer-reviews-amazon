# Predict-rating-based-on-customer-reviews-amazon
Steps:
1.	Importing libraries :
2.	Loading data of 28332 customers from excel. Use only reviews_text and eviews_rating column as features and labels respectively. Split data into train and test set. 19000 samples are used for training , rest for testing.
3.	Pre-processing data removing, hashtags, html tags, special characters, white spaces and converting to lower case
4.	To prepare text data for our deep learning model, we transform each review into a sequence. Every word in the review is mapped to an integer index and thus the sentence turns into a sequence of numbers.To perform this transformation, keras provides the Tokenizer
5.	Not all reviews are of same length. To handle this difference in length of reviews, we define a maximum length. For reviews which are smaller than this length, we pad them with zeros which longer ones are truncated
6. Build a neural network model. Compile and start the training.
97.61% accuracy was obtained on training set. 76.97% accuracy is obtained on test set. Confusion matrix drawn : labels are rating 1-5


