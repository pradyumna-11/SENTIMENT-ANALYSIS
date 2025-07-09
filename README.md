# SENTIMENT-ANALYSIS

"COMPANY" : CODTECH IT SOLUTIONS

"NAME" : SIKHAKOLLI PRADYUMNA

"INTERN ID" : CT08DN583

"DOMAIN" : DATA ANALYSIS

"DURATION" : 8 WEEKS

"MENTOR" : NEELA SANTOSH


## 📌 Task 4: Sentiment Analysis on Textual Data Using NLP

### 📝 Overview

The goal of this task is to **perform sentiment analysis** on textual data (such as reviews, tweets, or comments) using **Natural Language Processing (NLP)** techniques. Sentiment analysis, also known as opinion mining, is a key application of NLP that involves determining whether a given piece of text expresses a **positive**, **negative**, or **neutral** sentiment. This task is crucial in areas like customer feedback analysis, social media monitoring, and brand management.

In this task, we use Python libraries such as **NLTK (Natural Language Toolkit)** to process and analyze the sentiments of text samples using **VADER (Valence Aware Dictionary and sEntiment Reasoner)**—a lexicon and rule-based sentiment analysis tool specifically attuned to sentiments expressed in social media.

---

### 📂 Dataset

To simulate real-world data, a small sample dataset of textual entries (tweets and reviews) was created. Each text snippet reflects a different opinion, ranging from highly positive to extremely negative. Although the current sample is synthetic, this approach can easily be extended to real datasets fetched from Twitter, review platforms, or Kaggle datasets.

The dataset contains phrases like:

* “I love this product! It works amazingly well.”
* “Absolutely fantastic service, highly recommend!”
* “I hate it, waste of money.”
* “This is the worst experience I've ever had.”

This mix ensures a balanced evaluation across sentiment categories.

---

### ⚙️ Approach

1. **Text Processing**
   The text data is loaded into a pandas DataFrame. Each entry is passed to the VADER sentiment analyzer to extract sentiment polarity scores.

2. **Sentiment Scoring**
   VADER provides four scores for each text:

   * **Positive**: Probability of positive sentiment
   * **Neutral**: Probability of neutral sentiment
   * **Negative**: Probability of negative sentiment
   * **Compound**: A normalized score between -1 (most negative) and +1 (most positive)

3. **Categorization**
   Based on the `compound` score, each text is classified into:

   * **Positive** (compound ≥ 0.05)
   * **Negative** (compound ≤ -0.05)
   * **Neutral** (between -0.05 and 0.05)

4. **Visualization**
   A bar chart is created using **Seaborn** to visualize the distribution of sentiments across the dataset. This helps in identifying the proportion of positive, negative, and neutral opinions in the corpus.

---

### 📈 Results

Each input text is successfully assigned a sentiment label. The final output is a table displaying the original text, its compound score, and its classified sentiment. The accompanying bar chart clearly shows the sentiment trend in the data.

For example:

* “I love this product!” → Compound: 0.84 → **Positive**
* “This is the worst experience ever.” → Compound: -0.85 → **Negative**
* “Okay experience, nothing special.” → Compound: 0.0 → **Neutral**

---

### 🔍 Significance

Sentiment analysis provides actionable insights in many industries:

* **Businesses** can analyze customer feedback to improve services.
* **Marketers** can monitor brand sentiment on social media.
* **Product teams** can prioritize issues or features based on user emotion.

By automating this process using tools like VADER, organizations can make faster, data-driven decisions.

---

### 🚀 Future Enhancements

* Use larger, real-world datasets from Twitter API or product review sites
* Apply advanced models like **TextBlob**, **spaCy**, or **BERT transformers** for deeper analysis
* Implement a web-based interface to analyze text live
* Add preprocessing steps like stopword removal, stemming, and lemmatization

---

This task demonstrates the power of NLP and Python in understanding human language and transforming raw text into meaningful insights. It lays the foundation for more complex tasks such as emotion detection, topic modeling, and intent classification.


##Output:

<img width="1025" height="520" alt="Image" src="https://github.com/user-attachments/assets/1fb8feec-a9b1-4cff-9a51-f348e36c0bd8" />
