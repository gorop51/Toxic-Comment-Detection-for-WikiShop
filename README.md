# 🗣️ Toxic Comment Detection for WikiShop

## 📌 Project Overview

Developed a machine learning model for WikiShop, an e-commerce platform launching a wiki-style product description editing feature. The solution identifies toxic comments in user-generated content to streamline moderation processes and maintain a positive community environment.

## 🎯 Objective

Create a text classification model that:
- Accurately identifies toxic comments with F1 score ≥ 0.75
- Enables efficient content moderation by prioritizing potentially harmful content
- Handles significant class imbalance (only ~10% of comments are toxic)
- Processes natural language effectively through advanced text preprocessing

## 📊 Dataset Description

Labeled dataset of 159,292 user comments:
- **text**: User-generated comment content
- **toxic**: Binary target feature (1 = toxic comment, 0 = non-toxic)

## 🔍 Methodology

### Text Processing Pipeline
- Implemented comprehensive text cleaning (removing special characters, lowercasing)
- Applied lemmatization to normalize word forms
- Created effective text features using:
  - Unigrams (single word features)
  - TF-IDF vectorization for term importance weighting

### Model Development
- Addressed class imbalance through appropriate model selection and evaluation
- Tested multiple classification algorithms with hyperparameter tuning
- Implemented pipeline architecture for seamless text processing and classification
- Validated model performance against constant baseline to ensure meaningful results

## 📈 Results

**Model Performance**:
- Achieved F1 score of 0.773 (exceeding the 0.75 target)
- Significantly outperformed baseline model (0.10 F1 score)
- Successfully identified toxic content while minimizing false negatives

The solution enables WikiShop to automatically flag potentially harmful comments for human review, improving community safety while reducing moderator workload. The model's high performance ensures reliable detection of toxic content across diverse comment styles and linguistic patterns.
