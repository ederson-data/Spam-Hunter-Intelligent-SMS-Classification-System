SMS Spam Hunter: NLP & Machine Learning Project 🛡️
1. Project Overview
This repository contains the intelligence system developed for the Digital Communications Intelligence Unit (DCIU). The mission was to build a robust machine learning classifier to detect and flag SMS spam before it reaches users. Using Python and Natural Language Processing (NLP), this system identifies the "smoking guns" of phishing and spam messages with high accuracy.



2. Key Findings
Our exploratory data analysis revealed significant behavioral differences between legitimate (Ham) and fraudulent (Spam) messages:

The Length Factor: Spam messages are nearly double the length of legitimate messages, averaging 137.89 characters compared to 70.46 characters for "Ham".

Targeted Vocabulary: Fraudulent messages rely on high-urgency keywords such as 'Call' (303 occurrences), 'Free' (188), and 'Now' (156).

3. Data Preprocessing & Cleaning
To meet the rigorous standards of the DCIU field assignment, the following data pipeline was implemented:

Deduplication: Reduced the initial 5,572 records down to 5,169 unique messages to prevent model bias.

Normalization: All text was lowercased, stripped of punctuation, and filtered for common "stop words" to isolate the primary intent of the communication.

Vectorization: Utilized TF-IDF Vectorization to weigh the importance of specific keywords across the dataset.

4. Model Performance
The system uses a Multinomial Naive Bayes classifier, achieving the following metrics:

Overall Accuracy: 95%.

Spam Precision: 100% (Every message flagged as spam was correctly identified, ensuring zero false positives for critical business communications).


Spam Recall: 63% (The system is currently tuned to be conservative to avoid blocking legitimate messages).
