# Fine-Grained Topic Categorization of BBC News Articles

## About the Project

In today's digital world, thousands of news articles are published every day. Manually organizing them into categories can be difficult and time-consuming. This project focuses on solving that problem by using **Machine Learning and Natural Language Processing (NLP)** to automatically categorize news articles.

In this project, BBC news articles are analyzed and classified into different topics such as **Business, Entertainment, Politics, Sport, and Technology**. The model learns patterns from the text and predicts the most suitable category for each article.

To represent textual data in a meaningful way, the project uses **GloVe word embeddings**, which help capture the semantic meaning of words.

---

## Dataset

The dataset used in this project is the **BBC News Dataset**, which contains a collection of news articles along with their corresponding categories.

The dataset includes the following five topics:

* Business
* Entertainment
* Politics
* Sport
* Technology

Each article contains the full text and a label indicating its category.

---

## Project Process

The project follows a simple machine learning workflow:

1. **Loading the dataset**
   The BBC news dataset is loaded and explored.

2. **Text preprocessing**
   The raw text is cleaned to remove unnecessary characters and improve data quality.

3. **Word representation using GloVe**
   Words are converted into numerical vectors using pretrained GloVe embeddings.

4. **Model training**
   Different supervised machine learning models are trained using the processed data.

5. **Model evaluation**
   The models are tested and compared using performance metrics.

---

## Text Preprocessing

Before training the models, the text data is cleaned and prepared using common NLP techniques:

* Converting text to lowercase
* Removing punctuation and special characters
* Removing stopwords
* Tokenizing the text into words
* Lemmatizing words to their base form

These steps help improve the quality and consistency of the dataset.

---

## Word Embeddings with GloVe

Since machine learning models cannot directly understand text, the words need to be converted into numbers.

This project uses **GloVe (Global Vectors for Word Representation)**, a popular word embedding technique that represents words as numerical vectors based on their meaning and context.

For each article:

* Word embeddings are obtained for every word
* The vectors are averaged to create a single vector representation of the article
* This vector is used as input for the machine learning models

---

## Machine Learning Models Used

Several supervised learning algorithms were used to perform the classification task:

* **Decision Tree Classifier**
* **Gaussian Naive Bayes**
* **K-Nearest Neighbors (KNN)**
* **Radius Neighbors Classifier**

Each model was trained and tested to compare their performance.

---

## Evaluation Metrics

To understand how well the models perform, the following metrics were used:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

These metrics help evaluate how accurately the models classify the news articles.

---

## Tools and Technologies

This project was implemented using the following tools and libraries:

* Python
* Pandas
* NumPy
* Scikit-learn
* NLTK
* Matplotlib
* Seaborn
* WordCloud

---

## How to Run the Project

1. Clone the repository

```
git clone https://github.com/yourusername/bbc-news-classification.git
```

2. Install the required libraries

```
pip install pandas numpy scikit-learn nltk matplotlib seaborn wordcloud
```

3. Download and place the **GloVe embeddings** file in the project folder.

Example:

```
glove.6B.100d.txt
```

4. Run the Jupyter Notebook

```
BBC.ipynb
```

---

## Applications

This type of system can be useful in many real-world scenarios such as:

* Automatic news categorization
* News recommendation systems
* Content filtering platforms
* Information retrieval systems

---

## Conclusion

This project shows how **machine learning and NLP techniques** can be used to analyze and understand textual data. By combining **GloVe embeddings with supervised classification models**, it becomes possible to automatically categorize news articles and organize large collections of text efficiently.
