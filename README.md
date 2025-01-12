
# VeriGuard: Fake News Detection System

VeriGuard is a machine learning-based project that uses natural language processing (NLP) techniques to detect and classify news articles as real or fake. The system leverages text preprocessing techniques like stemming and TF-IDF vectorization, combined with a logistic regression model for accurate classification.

## Table of Contents
- [About](#about)
- [Technologies](#technologies)
- [Dataset](#dataset)
- [Setup](#setup)
- [Preprocessing](#preprocessing)
- [Model Training](#model-training)
- [Evaluation](#evaluation)
- [Accuracy](#accuracy)
- [License](#license)

## About

The goal of this project is to help identify fake news using machine learning and text analysis. The dataset contains news articles with labels indicating whether the news is real (0) or fake (1). This project demonstrates how NLP techniques can be applied to detect misinformation in the digital world.

## Technologies
- Python
- pandas
- numpy
- scikit-learn
- NLTK (Natural Language Toolkit)

## Dataset

The dataset consists of the following columns:
- **id**: Unique identifier for the news article
- **title**: Title of the news article
- **author**: Author of the news article
- **text**: Text of the article
- **label**: Label marking whether the news article is real (0) or fake (1)

## Setup

To set up this project, follow these steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/VeriGuard.git
   cd VeriGuard
   ```

2. Install the necessary dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the NLTK stopwords dataset by running the Python script included in the repository.

4. Place your dataset (e.g., `expanded_train.zip`) in the repository's root directory.

## Preprocessing

The dataset undergoes several preprocessing steps:
- Handling missing values
- Merging the title and text of each article to form a complete content
- Removing stopwords and non-alphabetical characters
- Applying stemming to reduce words to their root form

## Model Training

A logistic regression model is used to train the data after vectorizing the text content using TF-IDF. The model is then trained using an 80-20 split for training and testing.

## Evaluation

The model's accuracy is evaluated on both training and testing datasets.

### Accuracy:
- **Training Data Accuracy**: 97.12%
- **Test Data Accuracy**: 98.56%

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

This version of the README gives a high-level overview of your project without including the code.
