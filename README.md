# Shopping Predictor - CS50 AI Project

## Overview
This project implements a machine learning classifier to predict whether online shoppers intend to make a purchase based on their browsing behavior. The classifier uses a k-nearest neighbor algorithm (with k=1) to analyze user session data and determine purchase intent.

## Background
When users browse online shopping websites, only a fraction of them complete a purchase during their session. Being able to predict a user's purchasing intent can be valuable for e-commerce platforms, allowing them to customize the user experience (such as offering discounts to users who might not otherwise complete a purchase).

This project builds a nearest-neighbor classifier that analyzes various features of a user's browsing session to predict whether they will make a purchase. The classifier is trained on a dataset of approximately 12,000 user sessions from a shopping website.

## Features
The classifier analyzes the following features:
- Number of pages visited (Administrative, Informational, Product-related)
- Time spent on different page types
- Bounce rates and exit rates
- Special day proximity
- Page values
- Weekend vs. weekday visits
- Visitor type (returning or new)
- Browser and operating system information
- Region and traffic type

## Performance Metrics
The classifier's performance is measured using two key metrics:
- **Sensitivity** (True Positive Rate): The proportion of actual purchasers correctly identified
- **Specificity** (True Negative Rate): The proportion of non-purchasers correctly identified

## Project Structure
- `shopping.py`: Main implementation file containing the machine learning model
- `shopping.csv`: Dataset containing user session information and purchase outcomes

## Implementation Details
The project implements three main functions:
1. `load_data`: Loads and preprocesses the dataset from a CSV file
2. `train_model`: Trains a k-nearest neighbor classifier on the dataset
3. `evaluate`: Calculates sensitivity and specificity metrics for the model

## Requirements
- Python 3
- scikit-learn
- numpy (optional)
- pandas (optional)

## Usage
```
python shopping.py [shopping.csv]
```

## Credits
This project is part of CS50's Introduction to Artificial Intelligence with Python course offered by Harvard University.
