# Sentiment Analysis and Review Summarization on Amazon Food Products

## 📌 Project Overview
This project aims to analyze customer reviews of food products from Amazon. It includes sentiment classification (positive, neutral, negative) and automatic summarization using Natural Language Processing (NLP) models.

## 📂 Raw Dataset Link
- Dataset: Amazon Fine Food Reviews  
- Source: [https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews)  
- File used: `food.csv`

## 📊 Insight & Findings
- Majority of reviews are positive (score 4–5).
- Less than 20% of the reviews express negative sentiment (score 1–2).
- Most common positive keywords: *great*, *love*, *delicious*, *favorite*.
- Common negative themes involve *packaging issues* and *mislabeling*.

**Example of AI-generated summary:**

> Original Review:  
> “This saltwater taffy had great flavors and was very soft and chewy…”

> Summary:  
> *Great flavors and soft texture. Highly enjoyable!*

## 🤖 AI Support Explanation
This project uses pre-trained NLP models from the HuggingFace Transformers library:
- **Sentiment Classification**: `distilbert-base-uncased-finetuned-sst-2-english`
- **Summarization**: `facebook/bart-large-cnn`

These models are accessed via the `pipeline()` API, allowing quick implementation of AI-powered text analysis.
