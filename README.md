#  Sentiment Analysis Project

An end-to-end Artificial Intelligence project that classifies customer reviews into **Positive**, **Neutral**, or **Negative** categories using Natural Language Processing (NLP) and Machine Learning.

##  Project Overview
This project aims to automate the analysis of customer feedback for a fine food business. By identifying trends in customer sentiment, businesses can proactively address complaints and highlight popular products.

##  Dataset
- **Source**: [Sentimental Analysis (Google Colab)]( https://c32260f8eac749b956.gradio.live)
- **Features**: Review Text, Star Ratings (converted to Sentiment labels), and Review Length.

##  Tech Stack
- **Language**: Python
- **Libraries**: Pandas, Scikit-Learn, Matplotlib, Seaborn, Wordcloud, Scipy
- **Deployment**: Gradio (Web UI)

##  Key Findings (EDA)
- **Class Imbalance**: The dataset is heavily skewed toward positive reviews (~75%).
- **Length Pattern**: Negative reviews tend to have a higher word count, indicating that dissatisfied customers provide more detailed feedback.
- **Keywords**: Positive reviews are defined by words like  *'perfect'*, and *'highly'*, while negative reviews focus on *'disappointed'*, *'waste'*, and *'flavorless'*.

##  Model Building
- **Algorithm**: Logistic Regression with `class_weight='balanced'`.
- **Feature Engineering**: Combined **TF-IDF Vectorization** (Unigrams/Bigrams) with scaled **Review Length** features.
- **Tuning**: Grid Search was used to optimize the regularization parameter (C=1).
- **Evaluation**: The model achieved high F1-Scores across all classes, proving its reliability despite the data imbalance.

##  Deployment
The model is deployed via a **Gradio Web App**. Users can input custom text to receive a real-time sentiment prediction and confidence score.

### How to Run Locally:
1. Clone the repository:
   ```bash
   git clone [https://github.com/lynnchebby/Sentiment-Analysis-App.git](https://github.com/lynnchebby/Sentiment-Analysis-App.git)
