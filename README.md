# jigsaw_toxic_comment_classification

Given a group of sentences or paragraphs, which was used as a comment by a user in an online platform, the task is to classify it to belong to one or more of the following **six categories** - toxic, severe-toxic, obscene, threat, insult or identity-hate. This is a **multi-label classification problem**. In multi-label classification, data can belong to more than one label simultaneously. 

The evaluation metric is the mean column-wise **ROC AUC**. In other words, the score is the average of the individual AUCs of each predicted column.

Dataset from kaggle website: https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/

## PROJECT DESIGN & WORKFLOW

The project will comprise broadly the following steps:
### STEP 1: PREPROCESSING
• Convert each comment_text field to lower case letters

• Remove any punctuation marks (?!#,.etc)

• Using count vectorizer, generate a vector showing the frequency of each word in a
comment

• Divide the data into training and testing
### STEP 2: CREATING METHODS FOR EVALUATION METRICS
• find_accuracy

• find_hamming_loss
### STEP 3: WORKING WITH THE BENCHMARK MODEL (svm with radial kernel)
• Import the necessary files and create the model classifier

• Fit it to the training data using 5 fold cross-validation

• Predict using test data

• Calculate various evaluation metrics
### STEP 4: USING TRANSFORMATION METHODS
• Create a method for binary-relevance method using benchmark model as base classifier

• Create a method for either LP (Label Power Set) or CC(classifier chain)

• Fit classifier to training data

• Predict labels

• Calculate various evaluation metrics
### STEP 5: USING ADAPTATION ALGORITHMS
• Create classifiers for adaboost MH and MR models

• Try out different base classifiers for the above defined models

• Fit classifier to training data

• Predict labels and calculate various evaluation metrics
### STEP 6: IMPLEMENTING BP-MLL NEURAL NETWORKS
• Study and define the basic model architecture

• Compile your model using optimisers and accuracy as metric

• Run the model for certain epochs and batch size

• Calculate accuracy
### STEP 7: COMPILING RESULTS
• Compare the results for different models

• Decide which is the best model for given dataset
