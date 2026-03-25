# Sentiment Classification with BERT, DistilBERT, and Naive Bayes

A machine learning project that trains and benchmarks three NLP models on sentiment classification across multiple datasets. The goal was to understand the real-world tradeoffs between model complexity, accuracy, and speed.

## Authors

- Ayman Khan
- Mohammad Abbas
- Prashanth Babu

## Models Compared

| Model | Type | Notes |
|---|---|---|
| BERT | Transformer (full) | Highest accuracy, slowest to train |
| DistilBERT | Transformer (distilled) | Good accuracy with much faster training |
| Naive Bayes | Probabilistic baseline | Fast, interpretable, lower accuracy |

## Datasets

The models were trained and evaluated on three datasets:

- **Amazon Reviews** - product sentiment from customer reviews
- **Movie Reviews** - sentiment from film critique text
- **Restaurant Reviews** - sentiment from dining feedback

## Key Findings

- BERT achieved the highest accuracy across all datasets but required the most compute
- DistilBERT matched BERT closely at a fraction of the training time, making it the best tradeoff for most use cases
- Naive Bayes was the fastest by far and still competitive on simpler, shorter review text
- The performance gap between the models widened on longer, more nuanced text

## Getting Started

```bash
# 1. Clone the repo
git clone https://github.com/MohammadAbbas393/Sentiment-Classification-with-Naive-Bayes-Distillbert-and-Bert-main
cd Sentiment-Classification-with-Naive-Bayes-Distillbert-and-Bert-main

# 2. Install dependencies
pip install -r requirements.txt

# 3. Open the notebooks in Jupyter
jupyter notebook
```

## Requirements

- Python 3.8+
- PyTorch
- Transformers (HuggingFace)
- scikit-learn
- pandas
- numpy
- jupyter

Install with:

```bash
pip install torch transformers scikit-learn pandas numpy jupyter
```

## Project Structure

```
├── notebooks/
│   ├── bert_training.ipynb
│   ├── distilbert_training.ipynb
│   └── naive_bayes.ipynb
├── data/          # Dataset files
└── results/       # Saved model outputs and metrics
```

