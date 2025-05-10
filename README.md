# Decoding Emotions in Social Media Posts Using VADER

This project analyzes the emotional content of social media posts using sentiment analysis with the VADER (Valence Aware Dictionary and sEntiment Reasoner) tool. It classifies text into **Positive**, **Negative**, or **Neutral** sentiments and visualizes the results using pie charts.

## 📌 Project Overview

Social media is filled with emotional expressions — through words, emojis, slang, and punctuation. Manually understanding these emotions at scale is impossible. This project automates that process using VADER, a lexicon-based sentiment analysis tool designed for social media language.
![Image](https://github.com/user-attachments/assets/78e1d8b7-c9e0-460d-bbfd-62fdc99bc74d)

## 🎯 Objectives

- Preprocess Instagram post data (remove nulls, duplicates, retain emojis/punctuation).
- Classify sentiment using VADER compound scores.
- Visualize the sentiment distribution across social media platforms.
- Evaluate VADER's effectiveness vs. traditional ML models (planned for future).
- Ensure transparency, scalability, and ethical consideration in sentiment classification.

## 🧩 Dataset

- **Source**: [Open-source Instagram dataset from GitHub](#)
- **Format**: `Instagram-datasets.csv`
- **Records**: ~1000 Instagram posts
- **Target**: Generated via VADER during runtime (Positive, Neutral, Negative)

## ⚙️ Technologies Used

- **Python** 🐍
- **pandas** – Data manipulation
- **matplotlib** – Visualization
- **vaderSentiment** – Sentiment analysis

## 📊 Visual Results

The project analyzes multiple platforms (Facebook, Instagram, Twitter). Below are pie charts showing sentiment distributions:

### Facebook
![Image](https://github.com/user-attachments/assets/c4e6e175-db33-47f6-8f3e-b082d6ffb0b9)

### Instagram
![Image](https://github.com/user-attachments/assets/99c6e082-fdad-4165-ae2c-69ffb670c008)

### Twitter
![Twitter Output](Twitter_Output.png)

## 🚀 How It Works

1. Load the CSV dataset.
2. Preprocess data:
   - Remove duplicates and nulls.
   - Convert all text to string.
   - Retain emojis, capital letters, and punctuation.
3. Initialize the VADER Sentiment Analyzer.
4. Assign a sentiment score to each post:
   - **Score ≥ 0.5** → Positive
   - **Score ≤ -0.5** → Negative
   - **Otherwise** → Neutral
5. Aggregate sentiment counts.
6. Visualize using pie charts.

## 📈 Future Improvements

- Add supervised learning models for comparison (e.g., Logistic Regression, Naive Bayes).
- Include time-based or hashtag-based sentiment trends.
- Create word clouds for deeper insights.

## 👥 Team Members

- **Ranjith Kumar S** – Project planning, preprocessing, VADER integration, documentation
- **Purusothaman C** – Data sourcing, EDA, visualization
- **Sivaneshan S** – Feature engineering, sentiment labeling
- **Somasundaram D** – Multi-dataset testing, debugging, final documentation

## 📄 License

This project is for academic and research purposes under fair use. Contact authors for reuse in production.

## 📎 Repository

GitHub:https://github.com/Ranjith-Kumar-CSE/Sentiment-Analysis.git

