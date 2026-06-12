# MADT-8101-Customer-Analytics

![Python](https://img.shields.io/badge/python-3.8%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Last Commit](https://img.shields.io/github/last-commit/puwadonsri/MADT-8101-Customer-Analytics)
![Repo Size](https://img.shields.io/github/repo-size/puwadonsri/MADT-8101-Customer-Analytics)

> **Customer Analytics** — วิเคราะห์ข้อมูลลูกค้าครบวงจร ตั้งแต่การออกแบบ Data Platform, การคำนวณ CLV, การทำนาย Churn, การแบ่งกลุ่มลูกค้า ไปจนถึง Voice of Customer Analytics

---

## 📚 Syllabus

| #  | Chapter | Workshop | Notebook |
|----|---------|----------|----------|
| 1  | Overview of Customer Analytics | — | — |
| 2  | Designing Customer Data Platform | [WS1 ▶](./Workshop%201%20Customer%20Single%20View%20and%20Designing%20Customer%20Data%20Platform/) | [![Open](https://img.shields.io/badge/Notebook-01-blue)](notebooks/01_customer_single_view.ipynb) |
| 3  | Building Customer Single View | ↑ | ↑ |
| 4  | Basic Customer Analytics | — | — |
| 5  | Customer Lifetime Value | [WS2 ▶](./Workshop%202%20Customer%20Lifetime%20Value%20and%20Customer%20Scoring/) | [![Open](https://img.shields.io/badge/Notebook-02-blue)](notebooks/02_clv_scoring.ipynb) |
| 6  | Customer Scoring | ↑ | ↑ |
| 7  | Churn Scoring | [WS3 ▶](./Workshop%203%20Churn%20Scoring%20and%20Campaign%20Response%20Scoring/) | [![Open](https://img.shields.io/badge/Notebook-03-blue)](notebooks/03_churn_scoring.ipynb) |
| 8  | Campaign Scoring | ↑ | ↑ |
| 9  | Customer Segmentation | [WS4 ▶](./Workshop%204%20Customer%20Segmentation%20and%20Product%20Recommendation/) | [![Open](https://img.shields.io/badge/Notebook-04-blue)](notebooks/04_segmentation_recommendation.ipynb) |
| 10 | Segment Movement Analysis | ↑ | ↑ |
| 11 | Product Recommendation | ↑ | ↑ |
| 12 | Content Recommendation | — | — |
| 13 | Social Network Analysis | — | — |
| 14 | Voice of Customer | [WS5 ▶](./Workshop%205%20Voice%20of%20Customer%20Analytics/) | [![Open](https://img.shields.io/badge/Notebook-05-blue)](notebooks/05_voice_of_customer.ipynb) |

---

## 📓 Workshops

| Workshop | Topics |
|----------|--------|
| [1 — Customer Single View & CDP](./Workshop%201%20Customer%20Single%20View%20and%20Designing%20Customer%20Data%20Platform/) | ออกแบบ Customer Data Platform และสร้าง Customer Single View สำหรับบริษัท X Property |
| [2 — CLV & Customer Scoring](./Workshop%202%20Customer%20Lifetime%20Value%20and%20Customer%20Scoring/) | RFM Analysis, CLV Calculation, Customer Scoring Model, Spending Trend & Recency Analysis |
| [3 — Churn & Campaign Scoring](./Workshop%203%20Churn%20Scoring%20and%20Campaign%20Response%20Scoring/) | Churn Prediction (Random Forest), Campaign Priority Scoring, Feature Importance |
| [4 — Segmentation & Recommendation](./Workshop%204%20Customer%20Segmentation%20and%20Product%20Recommendation/) | K-Means Clustering, Segment Movement, Association Rules (Market Basket) |
| [5 — Voice of Customer](./Workshop%205%20Voice%20of%20Customer%20Analytics/) | Sentiment Analysis, LDA Topic Modeling, 3D Topic Visualization (Wongnai reviews) |

---

## 🚀 Quick Start

```bash
pip install -r requirements.txt
jupyter notebook
# Open notebooks/ folder and run any notebook
```

หรือเปิดใน Google Colab:
- [Workshop 5 — Colab Notebook](https://colab.research.google.com/drive/1soEu5T90lNPXTp8rstt0u7NyI0J2IWkX?usp=sharing)

---

## 🛠 Technologies

`Python` `Pandas` `Scikit-learn` `Matplotlib` `Seaborn` `NLTK` `LDA` `Jupyter`

---

## 📂 Project Structure

```
.
├── data/sample/               # Synthetic datasets for tutorials
├── notebooks/                 # Jupyter Notebooks (5 workshops)
├── Workshop 1 .../            # Workshop 1 — Customer Single View
├── Workshop 2 .../            # Workshop 2 — CLV & Scoring
├── Workshop 3 .../            # Workshop 3 — Churn & Campaign
├── Workshop 4 .../            # Workshop 4 — Segmentation
├── Workshop 5 .../            # Workshop 5 — Voice of Customer
├── .gitignore
├── requirements.txt
└── README.md
```

---

*MADT-8101 — Customer Analytics*
