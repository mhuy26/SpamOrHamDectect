# SpamOrHamDectection

## Spam SMS Detection
#### This project focuses on detecting spam SMS messages by analyzing a labeled dataset of SMS messages. The implementation follows the classic machine learning pipeline, using exploratory data analysis (EDA), text pre-processing, feature extraction, and classification to identify spam messages from legitimate ones.

### Data Preprocessing
The SMS messages are first cleaned and prepared for analysis. Text preprocessing includes:

Removing stopwords: We use the Python string module to filter out common words that do not carry significant meaning.
Removing punctuation: Punctuation is removed to ensure that the message contents are more easily comparable.
This ensures that only meaningful words are considered for feature extraction.

### Feature Extraction
We use the Bag of Words (BoW) method to represent the messages as numerical vectors, counting the occurrences of each word in each message.
To further refine this, we apply Term Frequency-Inverse Document Frequency (TF-IDF), which normalizes the word counts by giving less importance to common words that appear in many messages.

### Model Training
For the classification step, we use the Naive Bayes algorithm due to its simplicity and effectiveness for text classification tasks. Specifically, we implement the Multinomial Naive Bayes classifier from scikit-learn

### Model Fitting
Now, we fit the model and conclude classification report

### Other approach: 
We can create a pipeline. 
We will use SciKit Learn's [pipeline](http://scikit-learn.org/stable/modules/pipeline.html) capabilities to store a pipeline of workflow. This will allow us to set up all the transformations that we will do to the data for future use.
