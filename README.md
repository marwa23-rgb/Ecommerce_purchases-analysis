<h1 align="center">🛒 Ecommerce Purchases Analysis</h1>

<p align="center">
  Exploratory data analysis of 10,000 online purchase records using Python
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8-3776AB?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/Seaborn-Visualization-4C8CBF" alt="Seaborn">
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white" alt="Jupyter">
  <a href="https://www.kaggle.com/utkarsharya/ecommerce-purchases"><img src="https://img.shields.io/badge/Dataset-Kaggle-20BEFF?logo=kaggle&logoColor=white" alt="Kaggle"></a>
</p>

---

## 📑 Table of Contents

- [Overview](#-overview)
- [At a Glance](#-at-a-glance)
- [Workflow](#-workflow)
- [Key Findings](#-key-findings)
- [Visualizations](#-visualizations)
- [Repository Structure](#-repository-structure)
- [How to Run](#-how-to-run)
- [Next Steps](#-next-steps)
- [Author](#-author)

---

## 📌 Overview

This project explores the **Ecommerce Purchases** dataset from Kaggle. It cleans the data, answers 12 business-style questions with Pandas, and visualizes the results with Matplotlib and Seaborn.

---

## ⚡ At a Glance

| 🧾 Records | 🏷️ Avg. Purchase | 💰 Max Purchase | 🕐 AM / PM Split |
|:---:|:---:|:---:|:---:|
| **10,000** | **≈ $50.35** | **$99.99** | **4,932 / 5,068** |

---

## 🔄 Workflow

1. **Load & Inspect** – Reviewed the first and last rows, data types, and shape (`head()`, `tail()`, `dtypes`, `info()`).
2. **Clean** – Dropped `Address`, `Lot`, `CC Security Code`, and `IP Address`. Checked for missing values and duplicates: **none found**.
3. **Analyze** – Used filtering, `value_counts()`, and string operations to answer 12 questions.
4. **Visualize** – Built count plots and a bar chart with Seaborn.

> **Final dataset:** 10,000 rows × 10 columns  
> `AM or PM` · `Browser Info` · `Company` · `Credit Card` · `CC Exp Date` · `CC Provider` · `Email` · `Job` · `Language` · `Purchase Price`

---

## 🔍 Key Findings

| # | Question | Result |
|:---:|---|---|
| 1 | Average purchase price | **≈ $50.35** |
| 2 | Highest purchase price | **$99.99** (*Surveyor, hydrographic* and *Surveyor, insurance*) |
| 3 | Customers with French (`fr`) as language | **1,097** |
| 4 | Most common languages | German and Russian tie at **1,155**; Chinese is lowest at 1,059 |
| 5 | Job titles containing "engineer" | **984** |
| 6 | Mastercard users with purchases above $50 | **405** |
| 7 | Top credit card providers | **JCB 16 digit (1,716)** and **VISA 16 digit (1,715)** |
| 8 | Purchases in AM vs. PM | **PM: 5,068** · **AM: 4,932** |
| 9 | Cards expiring in 2020 | **988** |
| 10 | Top email domains | hotmail.com (1,638) · yahoo.com (1,616) · gmail.com (1,605) |
| 11 | Top browsers | **Mozilla (7,924)** · **Opera (2,076)** |
| 12 | Top 7 purchases | Prices from $99.92 to $99.99 (job and company in the notebook) |

---

## 📊 Visualizations

| Chart | Description |
|---|---|
| Count plot | Customers by language |
| Bar plot | Purchase price by credit card provider |
| Count plot | Purchases in the AM vs. PM |

<!-- To show the charts here, export them from the notebook (plt.savefig('language.png')),
     upload the PNGs to the repo, then add:
     <p align="center"><img src="language.png" width="600"></p> -->

---

## 📁 Repository Structure

```
├── Ecommerce Purchases.csv       # Dataset
├── Ecommerce_purchases.ipynb     # Analysis notebook
├── .gitignore
└── README.md
```

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/marwa23-rgb/Ecommerce_purchases.git
cd Ecommerce_purchases

# 2. Install the libraries
pip install pandas matplotlib seaborn jupyter

# 3. Open the notebook and run the cells in order
jupyter notebook Ecommerce_purchases.ipynb
```

---

## 🔮 Next Steps

- Analyze purchase price by job, company, or time of day
- Segment customers into groups with similar purchase habits (e.g., clustering)
- Build a simple dashboard of the main findings

---

## 👩‍💻 Author

**Marwa Samy** · [GitHub](https://github.com/marwa23-rgb)
