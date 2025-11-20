# Airbnb Data Mining & Sentiment Analysis Projects

*(Project 1 & Project 2 -- Data Mining Techniques)*

This repository contains two course projects completed for the
**Data Mining Techniques** course.\
Both projects use Airbnb data for Athens (2019 & 2023) and explore data
cleaning, visualisation, recommendation systems, sentiment analysis, and
word-embedding-based similarity metrics.

The work is implemented in Python through Jupyter Notebooks, following the specifications described in the official project descriptions.

## 📁 Repository Structure
```
    /
    ├─ project1/
    │  ├─ sdi2100275_sdi2100108.ipynb     # Jupyter notebook of project 1
    │  └─ Project_01_Description.pdf      # Project 1 instructions
    ├─ project2
    │  ├─ sdi2100275_sdi2100108.ipynb     # Jupyter notebook of project 2
    │  └─ Project_02_Description.pdf      # Project 2 instructions
    └─ README.md
```

# 📊 **Project 1 - Data Exploration & Recommendation System**

## **Part A - Data Exploration (Airbnb Athens 2019 & 2023)**

### ✔ Data preparation

-   Merge CSV files
-   Keep only required columns
-   Handle missing values and outliers
-   Clean & normalise fields such as `amenities`, `host_response_rate`,
    `price`, etc.

### ✔ Exploratory analysis

Includes: 
- Most common `room_type`
- Price evolution across months
- Top neighbourhoods by reviews
- Neighbourhood listing frequency
- Monthly distribution
- Heatmaps, histograms, distributions
- Most common room type per neighbourhood
- Most expensive room types
- Folium map visualising listings
- Wordclouds across multiple textual fields
- Grouping of amenities into simplified categories
- Neighbourhood price ranking & clustering
- Additional custom insights

## **Part B - Content-based Recommendation System**

### ✔ Components implemented

-   Text preprocessing
-   Stopword removal
-   Combined name + description field
-   **TF-IDF vectorization**
-   **Cosine similarity** matrix
-   Dictionary of top-100 similar listings
-   Recommendation function
-   Bigram collocations using `BigramCollocationFinder`

# 🤖 **Project 2 - Sentiment Analysis, Classification & Similarity Metrics**

## **Part 1 - Sentiment Annotation Using HuggingFace**

### ✔ Steps implemented:
-   Preprocessing of comments
-   Use of a HuggingFace model RoBERTa
-   Chunked annotation for 2019 & 2023
-   Production of datasets with columns:
    -   `id`
    -   `review`
    -   `sentiment`
-   Sentiment comparison over time

## **Part 2 - Classifier Training & Evaluation**

### ✔ Data Preparation

-   Train/test split (80/20%)
-   `train.tsv` & `test.tsv` datasets

### ✔ Feature Extraction

-   TF-IDF
-   Word embeddings
-   Stored using `pickle`

### ✔ Models Used

-   SVM
-   Random Forest
-   KNN

### ✔ Evaluation

-   10-fold cross-validation
-   Metrics: Accuracy, Precision, Recall, F1-score

## **Part 3 - Word Similarity & Semantic Neighbourhoods**

### ✔ Implemented tasks:

-   Word embeddings (trained or pre-trained)
-   Cosine similarity between words
-   For user-provided words + parameter N:
    -   Build a semantic neighbourhood
    -   Compute three similarities:
        1.  Maximum similarity of neighborhoods
        2.  Correlation of neighborhood similarities
        3.  Sum of squared neighborhood similarities
-   Visualization of neighbourhoods
-   Analysis of how similarity changes with N

---

# 📦 Technologies Used

-   Python
-   pandas, numpy
-   matplotlib
-   folium
-   wordcloud
-   scikit-learn
-   HuggingFace Transformers
-   NLTK
-   gensim
-   pickle
