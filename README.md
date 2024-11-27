
# Text Intensity Prediction Using NLP 
## Project Overview

This project aims to develop an intelligent system using Natural Language Processing (NLP) to predict the intensity of emotions (happiness, angriness, sadness) in text reviews. By analyzing textual data, the system provides insights into customer sentiment, enabling businesses to optimize processes and improve customer satisfaction.  



## Features

- Text preprocessing (e.g., lowercasing, removing stopwords, stemming, lemmatization).  
- Emotion intensity classification (happiness, angriness, sadness).  
- Feature extraction using TF-IDF vectorization and other linguistic features.  
- Machine learning models including Logistic Regression, Support Vector Machine, and more.  



## Workflow 
1. **Data Preprocessing**  
   - Text cleaning using libraries like `contractions`, `emoji`, and `nltk`.  
   - Lemmatization and stemming applied.  

2. **Feature Engineering**  
   - Extracted features include character count, word count, word density, polarity, and subjectivity.  
   - TF-IDF vectorization for high-dimensional text representation.  

3. **Model Training & Evaluation**  
   - Logistic Regression and SVM models trained.  
   - Metrics like accuracy, precision, recall, F1-score, and confusion matrix used for evaluation.  

## Prerequisites 
Install the dependencies using the `requirements.txt` file:  
```bash
pip install -r requirements.txt 
```
## Usage

Clone this repository.

Prepare your dataset in the data/ folder with files:

`happiness.csv`
`angriness.csv`
`sadness.csv`
Run the preprocessing and model training script.

Results will include metrics and predictions for test data.




## Result

The Support Vector Machine (SVM) model was chosen for its superior performance, achieving the highest accuracy of **79.22%** compared to other models like Logistic Regression (77.65%) and XGBoost (76.47%). It provided balanced precision and recall across all emotion categories, with fewer misclassifications as shown in the confusion matrix. The `rbf` kernel effectively handled non-linear relationships, ensuring robust predictions. SVM outperformed others, making it the optimal model for this task.
## Acknowledgements

Libraries used: `nltk`, `textblob`, `contractions`, `emoji`, `sklearn`, `xgboost`, `lightgbm`.
Dataset: Custom datasets for `happiness`, `angriness`, and `sadness`.