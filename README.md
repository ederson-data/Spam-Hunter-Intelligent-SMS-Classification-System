# Spam-Hunter-Intelligent-SMS-Classification-System
## 📖 Overview Recruited by the Digital Communications Intelligence Unit (DCIU), this project aims to protect users from the growing threat of mobile phishing and spam. Using Natural Language Processing (NLP) and Machine Learning, I built a classifier that identifies spam messages with a high degree of precision.
## 🎯 Project Objective
- Process and clean raw SMS data using Python and Regex.
- Convert text into numerical features using **TF-IDF Vectorization**.
- Train and evaluate **Naive Bayes** and **Logistic Regression** models.
- Analyze the linguistic differences between "Ham" (legitimate) and "Spam" messages.

## 🛠️ Tech Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
- **NLP Techniques:** Tokenization, Stop-word removal, TF-IDF Vectorization, Regex cleaning

## 📊 Key Results
The model achieved an overall **Accuracy of 96.32%**.

| Metric | Ham (Legitimate) | Spam |
| :--- | :--- | :--- |
| **Precision** | 96% | 100% |
| **Recall** | 100% | 71% |

**Key Insight:** The model achieved **100% Precision for Spam**, meaning it has a 0% false-alarm rate—no legitimate messages were accidentally blocked during testing.

## 📈 Insights & Findings
1. **The "Free" Factor:** The word "Free" is the #1 predictor of spam, appearing in nearly 40% of all spam messages.
2. **Message Length:** Spam messages are significantly longer on average (~140-160 characters) compared to ham messages, which are typically shorter conversational bursts.
3. **Zero False Positives:** The Naive Bayes model proved exceptionally safe for production as it never misclassified a "Ham" message as "Spam."
