# sentiment-analysis-on-product-reviews

# 🛍️ Sentiment Analysis on Product Reviews

> **Week 1 Project | AI & Data Analyst Internship**

An end-to-end Sentiment Analysis system that automatically reads e-commerce product reviews, classifies them as **Positive**, **Negative**, or **Neutral**, and generates meaningful business insights through data visualization.

---

## 📌 Problem Statement

E-commerce platforms receive thousands of customer reviews every day. Manually reading each review to understand customer satisfaction is **time-consuming and inefficient**.

This project solves that by building an automated sentiment analysis pipeline that:
- Reads and cleans raw product review data
- Applies NLP-based sentiment scoring to every review
- Classifies each review into Positive / Negative / Neutral
- Presents findings through charts and a written summary report

---

## 📁 Repository Structure

```
sentiment-analysis-on-product-reviews/
│
├── Sentiment_Analysis_on_Product_Reviews.ipynb   # Main Jupyter Notebook (all 5 tasks)
├── Dataset/                                       # Raw product reviews CSV dataset
├── Charts/                                        # All generated visualization charts
└── Summary.pdf                                    # Final insights & summary report
```

---

## ✅ Tasks Completed

### Task 1 — Data Loading & Exploration
- Loaded the CSV dataset using **Pandas**
- Displayed the first 10 rows to understand the structure
- Checked total number of rows and columns
- Identified the review text column for analysis

### Task 2 — Data Cleaning
- Removed rows where review text was **empty or null**
- Removed **duplicate reviews**
- Kept only the essential columns: **review text** and **rating/score**

### Task 3 — Sentiment Analysis
- Used the **TextBlob** library to calculate polarity score for each review
- Applied the following classification logic:
  - `score > 0` → **Positive**
  - `score < 0` → **Negative**
  - `score = 0` → **Neutral**
- Added a new `Sentiment` label column to the dataset

### Task 4 — Visualizations (3 Charts)
- **Chart 1 — Bar Chart:** Count of Positive, Negative, and Neutral reviews
- **Chart 2 — Pie Chart:** Percentage distribution of each sentiment category
- **Chart 3 — Custom Chart:** Creative visualization (e.g., rating vs sentiment comparison / most common words in negative reviews)

All charts are saved in the `Charts/` folder.

### Task 5 — Insights & Summary
Answered the following business questions inside the notebook:
- What percentage of reviews are positive?
- What do customers mostly complain about in negative reviews?
- What was surprising in the data?
- One actionable recommendation for the business

Full written summary available in [`Summary.pdf`](./Summary.pdf).

---

## 🛠️ Tools & Libraries Used

| Tool | Purpose |
|---|---|
| Python 3.x | Main programming language |
| Google Colab | Development environment |
| Pandas | Data loading and cleaning |
| TextBlob | Sentiment polarity analysis |
| Matplotlib / Seaborn | Charts and visualizations |

---

## 🚀 How to Run This Project

**1. Open in Google Colab**
 
Click the link below to open the notebook directly in Google Colab (no installation needed):
 
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/smohan-21/sentiment-analysis-on-product-reviews/blob/main/Sentiment_Analysis_on_Product_Reviews.ipynb)
 
**Or manually:**
1. Go to [colab.research.google.com](https://colab.research.google.com)
2. Click **File → Open Notebook → GitHub**
3. Paste this repo URL: `https://github.com/smohan-21/sentiment-analysis-on-product-reviews`
4. Select `Sentiment_Analysis_on_Product_Reviews.ipynb`
**2. Install required libraries** (run this cell first in Colab)
```python
!pip install textblob
```
 
**3. Download TextBlob language data**
```python
import nltk
nltk.download('punkt')
nltk.download('averaged_perceptron_tagger')
```
 
**4. Upload the dataset**
 
Upload the CSV file from the `Dataset/` folder when prompted, or mount your Google Drive:
```python
from google.colab import drive
drive.mount('/content/drive')
```
 
Run all cells from top to bottom to reproduce the full analysis.
 

---

## 📊 Key Outputs

- Cleaned dataset with sentiment labels added
- 3 visualizations saved in the `Charts/` folder
- Business insights written inside the notebook (Task 5)
- Summary report: [`Summary.pdf`](./Summary.pdf)

---

## 👤 Author

**Mohan S**
AI & Data Analyst Intern
GitHub: [@smohan-21](https://github.com/smohan-21)

---

## 📄 License

This project is built for internship and educational purposes.
