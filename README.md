# Spam-Classifier

• Trained a Multinomial Naive Bayes algorithm with data of 1000 messages resulting in 89.8% accuracy
• Using an add-one Laplace smoothing to handle unrealistic zero probabilities
• Taking the logarithms of posterior distributions to increase numerical stability


The training set consists of 1000 rows and 55 columns. Each row corresponds to one message. The first column is the response variable and describes whether a message is spam `1` or not `0`. The remaining 54 columns are features that are used to build a classifier. These features correspond to 54 different keywords (such as "money", "free", and "receive") and special characters (such as ":", "!", and "$"). A feature has the value `1` if the keyword appears in the message and `0` otherwise.

There is also a 500-row set of test data. It contains the same 55 columns.

The classifier takes input data and returns class predictions. The input is a single n*54 numpy array, the classifier returns a numpy array of length $n$ with classifications.
