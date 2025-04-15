# 🔍 Customer Sentiment Classifier

This project uses a pre-trained Transformer (DistilBERT) to classify customer feedback into sentiment categories. It is ideal for auto-labeling reviews, prioritizing support workflows, and detecting trends.

---

## 🧠 Project Summary
- 📊 **Problem**: Sentiment analysis on customer feedback
- 🧠 **Model**: `distilbert-base-uncased-finetuned-sst-2-english`
- 🏗️ **Tech Stack**: Python, Transformers (HuggingFace)
- 🎯 **Objective**: Score feedback as Positive or Negative with confidence scores

---

## 📁 Files

| File | Description |
|------|-------------|
| `05_sentiment_transformer.ipynb` | Loads DistilBERT and classifies 10 sample customer feedback texts |
| `data/customer_sentiment_reviews.csv` | Simulated dataset of reviews + ground truth sentiment labels |

---

## 📊 Dataset Features
- `customer_id`: Unique customer ID
- `text`: Customer feedback string
- `sentiment`: Labeled ground truth (`positive`, `neutral`, `negative`)

---

## ⚙️ How It Works
- Load HuggingFace pipeline with DistilBERT sentiment model
- Sample and score 10 reviews
- Print predictions and probabilities

---

## ✅ Example Output
```python
Text: Loved the experience!
 → Prediction: POSITIVE (0.98)
```

---

## 💡 Business Use Cases
- Auto-tag reviews for reporting dashboards
- Escalate negative feedback to human support
- Track changes in sentiment over product cycles

---

## 🔮 Next Steps
- Fine-tune model on company-specific review data
- Run classification on full dataset
- Visualize sentiment distribution over time

---
