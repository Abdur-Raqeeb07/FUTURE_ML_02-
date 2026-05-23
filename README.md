# 🎫 Support Ticket Classification System
### Future Interns — Machine Learning Track | Task 2
**Repository:** `FUTURE_ML_02`

---

## 📌 Objective
Build an NLP-based system to automatically classify customer support tickets into categories and assign priority levels, helping support teams respond faster and smarter.

---

## 🗂️ Ticket Categories

| Category | Description |
|---|---|
| Technical Issue | Bugs, crashes, server errors |
| Billing | Payments, charges, refunds, invoices |
| Account Access | Login, password, account lock/recovery |
| Feature Request | Suggestions and new feature ideas |
| General Inquiry | Questions, how-to, plan comparisons |

## ⚡ Priority Levels

| Priority | When Assigned |
|---|---|
| 🔴 High | Crashes, errors, unauthorized charges, account breaches |
| 🟡 Medium | Billing issues, access problems, incorrect data |
| 🟢 Low | Feature requests, general questions |

---

## 🛠️ Tools & Libraries

| Tool | Purpose |
|---|---|
| Python 3.10 | Core language |
| NLTK | Tokenization, stopword removal, lemmatization |
| Scikit-learn | TF-IDF vectorization, Logistic Regression, evaluation |
| Pandas | Data handling |
| Matplotlib / Seaborn | Visualizations |
| Google Colab | Development environment |

---

## 🔄 Pipeline Overview

```
Raw Ticket Text
      ↓
Text Preprocessing (lowercase → clean → tokenize → lemmatize → TF-IDF)
      ↓
Logistic Regression Classifier
      ↓
Category Prediction  +  Priority Tagging (rule-based)
      ↓
Output: { Category, Priority, Confidence Score }
```

---

## 📊 Key Features

- ✅ Text cleaning & tokenization (NLTK)
- ✅ TF-IDF vectorization with unigrams + bigrams
- ✅ Multi-class ticket category classification
- ✅ Priority tagging — High / Medium / Low
- ✅ Model evaluation — Accuracy, F1-score, Confusion Matrix
- ✅ Demo predictions on new unseen tickets

---

## 🚀 How to Run

1. Open [Google Colab](https://colab.research.google.com)
2. Go to **File → Upload Notebook**
3. Upload `FUTURE_ML_02_Support_Ticket_Classification.ipynb`
4. Click **Runtime → Run All**

No additional setup needed — all dependencies are installed in the first cell.

---

## 📁 Files

| File | Description |
|---|---|
| `FUTURE_ML_02_Support_Ticket_Classification.ipynb` | Main notebook — full pipeline |
| `README.md` | Project documentation |

---

## 📈 Sample Results

| Ticket | Category | Priority | Confidence |
|---|---|---|---|
| App crashes on PDF export | Technical Issue | 🔴 High | ~34% |
| Charged twice, need refund | Billing | 🔴 High | ~44% |
| Forgot password, reset not arriving | Account Access | 🟡 Medium | ~43% |
| Please add Gantt chart view | Feature Request | 🟢 Low | ~50% |
| Difference between pro and enterprise | General Inquiry | 🟢 Low | ~32% |

> Confidence scores are moderate due to the small synthetic dataset (200 tickets). A larger real-world dataset would significantly improve scores.

---

## 🔮 Future Improvements

- Use a real-world dataset (Kaggle support ticket datasets)
- Try SVM, Random Forest, or fine-tuned BERT for higher accuracy
- Train a separate ML model for priority classification
- Deploy as a REST API using FastAPI or Flask

---

**Future Interns | Machine Learning Internship | Task 2**
