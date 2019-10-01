# jigsaw_toxic_comment_classification

Given a group of sentences or paragraphs, which was used as a comment by a user in an online platform, the task is to classify it to belong to one or more of the following **six categories** - toxic, severe-toxic, obscene, threat, insult or identity-hate. This is a **multi-label classification problem**. In multi-label classification, data can belong to more than one label simultaneously. 

The evaluation metric is the mean column-wise **ROC AUC**. In other words, the score is the average of the individual AUCs of each predicted column.

Dataset from kaggle website: https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/

The baseline model is using logistic regression model, which gains the final score 0.97421.
The improved model is using LSTM deep learning model, which gains the final score 0.97233.

## PROJECT DESIGN & WORKFLOW

The project will comprise broadly the following steps:
### STEP 1: Read Training and Test Files

### STEP 2: Exploraty Data Analysis

• Dimensions of the data set

• Completeness of data set (missing values checking)

• Calculate and add 'clean' (the comments are not in any toxic categories) as new column

• Identify the distribution of labels

• Characters and words number statistics

### STEP 3: Data Cleaning

• Check the normal alphabet and to figure out the abnormal special characters

• Clean and remove some meaningless messy characters

• Normalization: convert the comments to lower cases

### STEP 4: Model Building

• Define the basic model architecture

• Compile the model using optimisers and accuracy as metric

• Run the model for certain epochs and batch size

### STEP 5: COMPILING RESULTS
• Compare the results for different models

• Decide which is the best model for given dataset
