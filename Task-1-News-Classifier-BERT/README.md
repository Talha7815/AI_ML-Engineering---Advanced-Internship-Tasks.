# Task 1: News Topic Classifier Using BERT

## Objective
Fine-tune a transformer model (BERT) to classify news headlines into topic categories.

## Dataset
AG News Dataset (Hugging Face Datasets)

## Methodology
- Tokenized and preprocessed the AG News dataset
- Fine-tuned bert-base-uncased model using Hugging Face Transformers
- Evaluated model using accuracy and F1-score
- Deployed model using Streamlit for live interaction



## Files
- `news_classifier_bert.ipynb` - Jupyter notebook with complete implementation
- `app.py` - Streamlit deployment script
- `requirements.txt` - Dependencies

## How to Run
1. Install dependencies: `pip install -r requirements.txt`
2. Run notebook: `jupyter notebook news_classifier_bert.ipynb`
3. Launch app: `streamlit run app.py`
