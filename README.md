# Amazon Product Reviews Sentiment Analysis using Python

## 📌 Project Overview

This project focuses on **Sentiment Analysis of Amazon Product Reviews** using Natural Language Processing (NLP) and Machine Learning techniques.

The objective is to classify customer reviews into two sentiment categories:
- **Negative Sentiment (0):** Reviews with ratings of 1, 2, or 3.
- **Positive Sentiment (1):** Reviews with ratings of 4 or 5.

A Logistic Regression classification model is trained using TF-IDF (Term Frequency-Inverse Document Frequency) features to predict the sentiment of customer reviews.

## 🎯 Objectives

- Analyze customer reviews from Amazon products.
- Perform text preprocessing and cleaning.
- Convert textual reviews into numerical features using TF-IDF.
- Visualize positive and negative sentiments using WordClouds.
- Build a sentiment classification model using Logistic Regression.
- Evaluate model performance using accuracy and a confusion matrix.

## 🛠️ Technologies & Libraries Used

- **Python** – Programming language
- **Pandas** – Data manipulation and analysis
- **NLTK** – Natural Language Processing
- **Scikit-learn** – Machine Learning and model evaluation
- **Matplotlib** – Data visualization
- **WordCloud** – Text visualization

## 📂 Dataset

**Dataset:** Amazon Product Reviews Sentiment Analysis Dataset

The dataset contains customer reviews and their corresponding sentiment ratings.

The following columns are used:
- `Review`: Textual customer reviews.
- `Sentiment`: Customer rating ranging from 1 to 5.

The sentiment labels are converted into binary classification:

| Original Rating | Sentiment Label | Category |
|---|---|---|
| 1, 2, 3 | 0 | Negative |
| 4, 5 | 1 | Positive |

## ⚙️ Project Workflow

### 1. Importing Libraries

Import the required Python libraries for data processing, NLP, visualization, and machine learning.

### 2. Data Loading and Exploration

- Load the Amazon reviews dataset using Pandas.
- Explore the dataset using `head()` and `info()`.
- Remove missing values using `dropna()`.

### 3. Sentiment Label Conversion

Convert the original sentiment ratings into binary labels:

- Ratings less than or equal to 3 are classified as negative (0).
- Ratings greater than 3 are classified as positive (1).

### 4. Text Preprocessing

Clean customer reviews by removing English stopwords using the NLTK stopwords corpus.

### 5. Exploratory Data Analysis

Generate separate WordCloud visualizations for:
- Negative customer reviews.
- Positive customer reviews.

These visualizations help identify frequently occurring words in each sentiment category.

### 6. Feature Extraction using TF-IDF

Use `TfidfVectorizer` to convert textual reviews into numerical feature vectors.

The model uses the 2,500 most relevant text features.

### 7. Train-Test Split

Split the dataset into training and testing sets:

- Training data: 75%
- Testing data: 25%
- Random state: 42

### 8. Model Building

Use **Logistic Regression** as the machine learning classification algorithm.

Train the model using the training dataset and predict sentiment labels for the test dataset.

### 9. Model Evaluation

Evaluate model performance using:

- Accuracy Score
- Confusion Matrix

The confusion matrix helps visualize the model's classification performance for positive and negative reviews.

## 📊 Results and Visualizations

The project generates the following visualizations:

1. Negative Sentiment WordCloud
2. Positive Sentiment WordCloud
3. Confusion Matrix

The Logistic Regression model is evaluated using accuracy on the test dataset.

**Model Accuracy:** Run the notebook or Python script to obtain the actual accuracy score.

## 👩‍💻 Author

**Athira Mohan**

## ⭐ Acknowledgements

- Scikit-learn documentation
- NLTK documentation
- Pandas documentation
- Amazon Product Reviews Dataset

---

If you find this project useful, don't forget to ⭐ the repository!
