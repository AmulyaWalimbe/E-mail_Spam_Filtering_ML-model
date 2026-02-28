# E-mail_Spam_Filtering_ML-model
Email spam filtering is the process of automatically identifying and removing unwanted or unsolicited emails (also known as spam) from a user's email inbox. The dataset used consists of examples of both spam and ham mails. Here the independent variable is the ‘Message’ and dependent is whether it is ‘spam’ or ‘ham’ that is ‘Category’. The input will be given as a message and the model thus predicts whether it is spam or ham mail.

1) Background and Overview
Email is one of the most popularly used communication mediums, but the presence of spam emails is affecting productivity, creating security hazards, and putting the user at the receiving end of phishing attacks.
The objective of this project is to create a supervised learning model for classifying emails into Spam or Not Spam (Ham).

Objective: To create a model for accurate spam detection with the least number of false positives and false negatives.

2) Data Structure Overview
The dataset consists of labeled email messages with:
•	Text column – raw email content
•	Label column – spam (1) or ham (0)
 
Preprocessing steps include:
•	Replaced missing values with empty strings to ensure clean text input
•	Converted categorical labels (“ham” and “spam”) into numerical format (0 and 1)
•	Applied TF-IDF vectorization within a Scikit-learn pipeline, which:
•	Lowercased text automatically
•	Tokenized email content
•	Removed punctuation
•	Converted text into numerical feature vectors
Used a Pipeline to ensure consistent preprocessing during both training and prediction (preventing data leakage).
The final dataset is transformed into a structured matrix suitable for classification modeling.
 

3) Executive Summary
The performance of the Spam Classifier, based on models like Naïve Bayes and Logistic Regression, was very good in metrics like accuracy, precision, recall, and F1 score.
          
Out of which Naïve Bayes has a slightly better overall performance, so selected that as the final model.
 
Key Outcome:
•	High Spam Detection Rate
•	Controlled False Positive Rate
•	Balanced Precision-Recall Tradeoff

4) Insights Deep Dive
•	Spam emails frequently contain repeating promotional words and words related to urgency. 
•	Legitimate emails tend to display more structural characteristics related to context. 
•	Accuracy is a vital factor, as misclassifying a positive is more problematic than misclassifying spam. 
•	Text preprocessing plays an important role in improving text classification. 
•	The evaluation of the model highlighted that minimizing misclassification costs is more important than maximizing accuracy. 

5) Recommendations
•	The model should be used with a spam folder that allows users to review spam emails to avoid any information loss. 
•	The model should be retrained with new data to keep up with new spam trends. 
•	The model's fairness with different writing styles and language differences should be kept in mind. 
•	The use of Explainable AI can be explored further.

