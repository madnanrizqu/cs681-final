## Description

This project explores the application of transformer models to two natural language processing tasks: text summarization and sentiment analysis.

**1. Text Summarization:**
- This part focuses on fine-tuning Microsoft's Phi-2 large language model (LLM) for text summarization.
- The model is trained on the CNN Dailymail dataset.
- The performance of the fine-tuned Phi-2 model is compared against the baseline Phi-2 model (without fine-tuning).
- Evaluation metrics: ROUGE, BLEU, and perplexity.
- Notebook: `cs681-final/summarization/main.ipynb`

**2. Sentiment Analysis:**
- This part explores the fine-tuning of DistilBERT for sentiment analysis.
- The model is trained on the sst2 dataset.
- The performance of the fine-tuned DistilBERT is compared against a baseline DistilBERT (without fine-tuning) and a Support Vector Machine (SVM) model.
- Evaluation metrics: accuracy, precision, recall, and f1-score.
- Notebook: `cs681-final/sentiment-analysis/main.ipynb`

## How to run notebooks

### Requirements:
- Python 3.11.11
- For the summarization notebook (`cs681-final/summarization/main.ipynb`), it is tested to run on a Kaggle GPU P100 environment.
- For the sentiment analysis notebook (`cs681-final/sentiment-analysis/main.ipynb`), ensure all packages listed in its `requirements.txt` are installed.

### Steps:

**For Text Summarization:**
1. Ensure you have the required Python version and a Kaggle GPU P100 environment.
2. Open the `cs681-final/summarization/main.ipynb` notebook.
3. Run the cells in the notebook sequentially.
   The notebook will:
    - Load configurations (model, dataset, training parameters).
    - Preprocess the CNN Dailymail dataset.
    - Fine-tune the Phi-2 model.
    - Evaluate the fine-tuned model and the baseline model.
    - Display the results.

**For Sentiment Analysis:**
1. Ensure you have the required Python version and have installed all necessary packages (see `requirements.txt` within the `sentiment-analysis` directory or the notebook's initial cells for package installation).
2. Open the `cs681-final/sentiment-analysis/main.ipynb` notebook.
3. Run the cells in the notebook sequentially.
   The notebook will:
    - Load and preprocess the sst2 dataset.
    - Fine-tune the DistilBERT model.
    - Train a baseline SVM model.
    - Evaluate the fine-tuned DistilBERT, baseline DistilBERT, and SVM model.
    - Display the comparison results.
