# 📊 Market Traction Segmentation and Intervention Prioritization in True Wireless Earphones

**An Unsupervised Learning Analysis Based on Observable Market Signals**

---

## 📌 Overview

E-commerce platforms host large product catalogs where **observable market behavior** varies across price levels, user ratings, and cumulative engagement. When direct information on **sales, exposure, or product lifecycle stage** is unavailable, publicly observable signals can be used to examine **relative market traction**.

This project applies **unsupervised learning techniques** to segment **true wireless earphones listed on Flipkart** using **price variables, cumulative review volume, and user ratings**, with the aim of identifying products that exhibit **relatively weaker observable market traction** and may require closer monitoring or intervention.

---

## 🎯 Business Problem

When only public signals are available:

> **Which products currently visible on the platform exhibit relatively weaker observable market traction and may require closer monitoring or intervention?**

Low observable traction does **not necessarily imply poor product quality**. It may reflect under-exposure, weak discoverability, or early lifecycle stages. This analysis focuses on structuring such signals to support **evidence-based intervention prioritization**.

---

## 🧠 Objectives

* Segment true wireless earphones based on **observable market signals**
* Identify segments with **relatively weaker observable market traction**
* Examine whether weak signals align more with **under-exposure** or **structural weaknesses**
* Support **monitoring and intervention prioritization** using unsupervised learning

---

## 🗂 Dataset Description

* **Dataset:** Flipkart Earphones
* **Source:** Kaggle (pre-crawled Flipkart listings)
* **Scope:** Only **true wireless earphones** retained for comparability

### Variables Used

* Offer price
* Real price
* User ratings
* Cumulative review count

These variables act as **proxies** for price level, perceived quality, and engagement.

---

## ⚙️ Methodology

* Data cleaning and preprocessing
* Log transformation of skewed variables (prices, reviews)
* Feature standardization for distance-based methods
* **Elbow method** to suggest cluster count
* **Hierarchical clustering (Ward linkage)** to *validate* cluster structure
* **K-Means clustering** for final segmentation
* Interpretation using:

  * Pairwise feature-space analysis
  * Cluster-wise summary statistics
  * Principal Component Analysis (PCA)

---

## 📈 Key Results

* Products form **four overlapping clusters**
* Market traction is **continuous and multidimensional**
* Two clusters exhibit **relatively weaker observable market traction**, driven primarily by **low cumulative engagement**
* Weak traction **cannot be inferred from price or ratings alone**

Clusters represent **relative monitoring and investigation priority groups**, not definitive performance labels.

---

## 🧭 Strategic Implications

* **Higher-rated but low-engagement products**
  → Possible under-exposure; suitable for monitoring and visibility-oriented experiments

* **Higher-priced, low-engagement products with lower ratings**
  → Candidates for deeper diagnostic review (pricing, positioning, customer feedback)

Ongoing monitoring of review accumulation and rating dynamics is critical to distinguish early-stage products from persistent low-traction offerings.

---

## 🗃 Repository Structure

```
├── Market Traction Segmentation and Intervention Prioritization in True Wireless Earphones (Report).pdf
├── Market_Traction_Segmentation_and_Intervention_Prioritization_in_True_Wireless_Earphones_(Notebook).ipynb
├── README.md
└── earphones.csv
```

---

## 🛠 Tools Used

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib
* Seaborn

---

## ⚠️ Limitations

* Only **publicly observable signals** are used
* No access to sales, exposure, or product age
* Review counts are cumulative (no temporal dynamics)
* Distance-based clustering imposes geometric assumptions

Results should be interpreted **relatively, not causally**.

---

## 🔮 Future Scope

Future work may incorporate **product age, exposure, and time-series review trends** to distinguish early-stage products from structural underperformers. Integrating **sales and conversion metrics**, expanding feature sets, and developing **monitoring or predictive models** could enable more proactive intervention planning.

---

## ✅ Conclusion

This study demonstrates how **unsupervised learning** can structure limited observable market data into interpretable segments that highlight products with **relatively weaker observable market traction**. The analysis emphasizes that traction is **multidimensional and overlapping**, and that careful, context-aware interpretation is essential when working under public-data constraints in real e-commerce settings.

---

## 👩‍💻 Author

**Sohini Mandal**

---
