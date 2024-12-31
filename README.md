# Fake News Detection System

## Overview
This project addresses the growing issue of misinformation by developing a machine learning-based system to classify news articles as real or fake. The system leverages natural language processing (NLP) techniques to analyze and extract meaningful features from textual content, using a Random Forest classifier to achieve accurate predictions.

---

## Features
- **Text Preprocessing**: Cleans and standardizes the input text, including removing special characters, lowering case, and removing stopwords.
- **Feature Extraction**:
  - Title and text length analysis.
  - Keyword density for sensational words.
  - Sentiment analysis for headlines and articles.
- **Machine Learning Model**: Employs a Random Forest classifier for efficient and accurate classification.
- **Evaluation Metrics**: Measures model performance using:
  - Accuracy
  - Precision
  - Recall
  - F1 Score
  - ROC-AUC

---

## Technologies Used
- **Python**: Core programming language.
- **Pandas & NumPy**: For data manipulation and numerical computations.
- **Scikit-learn**: For machine learning model implementation and evaluation metrics.
- **NLTK**: For natural language processing tasks like sentiment analysis.
- **TF-IDF**: For text vectorization and feature extraction.

---

## How to Run
### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/FakeNewsDetection.git
cd FakeNewsDetection
```

### 2. Install Dependencies
Install the required Python libraries:
```bash
pip install -r requirements.txt
```

### 3. Update Dataset Paths
Ensure the paths for the training and test datasets are correctly specified in the script.

### 4. Run the Script
Execute the script to train the model and classify the test data:
```bash
python fake_news_detection.py
```

---

## Dataset
The project requires a dataset containing the following columns:
- `title`: Headline of the article.
- `text`: Main content of the article.
- `label`: Binary label indicating whether the article is real (1) or fake (0).

Ensure the dataset is in CSV format and follows the expected structure.

---

## Results
The model achieves the following metrics on the evaluation set:
- **Accuracy**: 0.99
- **Precision**: 0.99
- **Recall**: 0.99
- **F1 Score**: 0.99
- **ROC-AUC**: 1

Results for the test dataset are saved in `results.csv` in the following format:
```csv
"title","predicted_label"
"Trump's new policy reviewed",1
"Shocking claims about health!",0
```

---

## Future Improvements
- Incorporate advanced language models like **BERT** for contextual understanding.
- Expand the dataset to improve generalization.
- Add temporal analysis to detect patterns during major events like elections.

---


## Acknowledgements
Special thanks to the contributors and the dataset providers for making this project possible.

