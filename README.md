# 🧠 Sentiment Analysis of Amazon Product Reviews

## 📖 Project Overview
This project focuses on sentiment analysis of Amazon customer reviews to determine whether product feedback is positive, neutral, or negative. Using Natural Language Processing (NLP) techniques with the spaCy library, the goal was to process real-world text data, clean it, and analyze sentiment patterns across customer reviews.

The dataset used — `Datafiniti_Amazon_Consumer_Reviews_of_Amazon_Products_May19.csv` — contains verified Amazon reviews, including the review text, ratings, and submission dates. This project demonstrates the process of building a simple NLP pipeline for sentiment analysis and evaluating its accuracy on sample inputs.

## 🛠️ Tools & Libraries
- **Python**
- **spaCy** (en_core_web_md)
- **pandas**
- **TextBlob**
- **NumPy**

## 🧹 Data Preprocessing
To prepare the dataset for analysis, the following steps were implemented in Python:

- **Data Extraction**: Selected the "reviews.text" column, which contains the written customer feedback.
- **Handling Missing Values**: Removed all missing or null values using `dropna()` from pandas.
- **Text Cleaning**:
  - Converted all text to lowercase.
  - Removed stop words, punctuation, numbers, and non-alphabetic characters.
  - Tokenized and stored cleaned sentences in a new column for analysis.

These preprocessing steps ensured the data was clean, consistent, and ready for sentiment classification.

## ⚙️ Model Development
- The `en_core_web_md` model from spaCy was used to enable Natural Language Processing tasks such as tokenization, vectorization, and part-of-speech tagging.
- A sentiment analysis function was developed to take a product review as input and classify its sentiment based on the polarity of the text.
- This function was then tested on multiple sample reviews to validate its performance.

## 📊 Results & Evaluation
After testing the model on several reviews:
- **2 out of 4 reviews** were correctly classified as positive.
- **2 out of 4 reviews** were classified as neutral.

These results indicate that the sentiment analysis function performed well at detecting positive sentiment, though more advanced models could yield finer distinctions in emotion and context.

## 💡 Insights

### ✅ Strengths
- Efficient and fast text cleaning and processing.
- Automated sentiment detection without the need for large training data.
- Accurate for general polarity (positive/neutral/negative).

### ⚠️ Limitations
- Lacks contextual understanding: Models like TextBlob and spaCy base sentiment on surface-level word meaning, so sarcasm or mixed sentiment may be misclassified.
- Non-adaptive: The rule-based model does not learn from new data like machine learning models do.

## 🏁 Accomplishments
Through this project, I successfully:
- Loaded and explored a real-world Amazon reviews dataset.
- Preprocessed and cleaned raw text data for NLP.
- Implemented a Python-based sentiment analysis pipeline using spaCy and TextBlob.
- Created and tested a custom sentiment prediction function.
- Generated a summary report (`sentiment_analysis_report.pdf`) detailing methodology, evaluation, and insights.
