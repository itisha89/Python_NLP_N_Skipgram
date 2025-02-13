# Word Embeddings and Similarity Analysis on Airline Reviews

## Dataset
The dataset used in this project is downloaded from Kaggle:
[Airline Reviews Dataset](https://www.kaggle.com/datasets/chaudharyanshul/airline-reviews)

## Project Overview
The project focuses on natural language processing (NLP) techniques applied to airline reviews. We explore word embeddings using the Skip-gram Word2Vec model and apply various text preprocessing techniques such as:

- **Trigram Generation**
- **Stemming & Lemmatization**
- **Word Embeddings using Skip-gram Word2Vec Model**
- **Similarity Analysis using Cosine Similarity**
- **Dimensionality Reduction using PCA**

## Observations

### Identifying Similar Words
To identify the top five similar words with significant similarity, we use a similarity metric like **cosine similarity** on the vectorized representations of words. This helps in understanding semantic relationships between words.

### Dimensionality Reduction for Visualization
To visualize word embeddings in a **2D semantic space**, **Principal Component Analysis (PCA)** is applied. PCA helps in reducing the dimensionality while preserving important relationships among words.

### Cosine Similarity in Word2Vec
Cosine similarity is implicitly used when obtaining similarity scores from the Word2Vec model. It is a common metric for measuring similarity between vectors in high-dimensional spaces, particularly in the context of word embeddings. The following key points justify its use:
1. **Cosine similarity measures the cosine of the angle between two vectors**—capturing semantic similarity rather than magnitude.
2. **It is invariant to vector magnitudes**, making it well-suited for NLP tasks.

### Implementation Details
The project includes functions that:
- Iterate through a list of words (`word_to_check`).
- Identify the **top 5 similar words** using the trained **Word2Vec model**.
- Compute **similarity scores** between words using cosine similarity.

This provides insights into the relationships between words based on the trained Word2Vec model.

## Design Techniques Used
1. **Word Embeddings**: Trained using the **Word2Vec Skip-gram model (w2v_model_sg)**.
2. **Vectorized Representations**: Words are transformed into vectors representing their semantic meaning.
3. **PCA Dimensionality Reduction**: Used to reduce the feature space and visualize word embeddings in 2D.
4. **Top Similar Words Identification**: The model identifies and prints the top **N similar words** based on cosine similarity scores.

## Conclusion
These techniques allow for a meaningful representation of words in a reduced dimensional space, making it easier to interpret semantic similarities and differences between words in airline reviews.

## 🌍 Explore More Projects  
For more exciting machine learning and AI projects, visit **[The iVision](https://theivision.wordpress.com/)** and stay updated with the latest innovations and research! 🚀  

---
