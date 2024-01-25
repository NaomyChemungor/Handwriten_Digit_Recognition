# Handwriten_Digit_Recognition
### Supervised Machine Learning k-Nearest Neighbors(k-NN) & Naive Bayes Classifier Algorithms to essentially a multiclass classification task

#### Further Details on important steps taken

##### Preprocessing
* Loading MNIST dataset, split into training and testing sets using TensorFlow
* Normalize pixel values in range -1 to 1 for balanced features
* Flattening images to 1D for efficient matrix multiplications in TensorFlow
* Selecting digits for classification, filter training and test data accordingly
  
##### k-NN Algorithm
* Defining k-NN prediction function with parameters
* Iterating through test data using a for loop.
* Calculating Euclidean distances, sort, get labels, predict, and append results
* Make predictions using KNN function with specified neighbors in this case it was set to 7,(adviceable to choose odd number to avoid a tie)

    * Note that unlike many algorithms, k-NN skips formal training; it uses the training data directly, remembering patterns without a separate training phase.
 
 * Evaluating prediction k-NN using accuracy,confusion matrix and f1-score

##### Naive Bayes Classifier Algorithm
  * Creating Naive Bayes classifier to calculate class and feature probabilities
  * Training the classifier using the provided dataset
  * Predicting classes for each sample in the test dataset
  * Calculating accuracy by comparing predicted and true labels
  * Instantiating the Naive Bayes classifier
  * Training the classifier using the flattened training data (X_train_flat, y_train)
  * Evaluating prediction for Naive Bayes Classifier using accuracy,confusion matrix and f1-score


