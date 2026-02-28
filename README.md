# Customer Segmentation, Financial Risk & Sentiment Analysis  
**Poshem Technology Institute – Data Challenge**

## Overview

This project explores **unsupervised customer segmentation and financial behaviour analysis** using a combination of **machine learning and NLP techniques**. It was developed as part of the Poshem Technology Institute Data Challenge and is inspired by real-world challenges faced by financial institutions across African markets.

In many emerging economies, customer financial behaviour is difficult to model due to incomplete financial histories, informal income sources, rapid growth in digital payment channels, and large volumes of unstructured customer feedback. Traditional credit scoring systems often fail to capture these realities.

This project addresses the gap by using **data-driven clustering and text analysis** to uncover natural customer segments, behavioural trends, and early indicators of potential financial risk—without relying on predefined labels.

---

## Problem Focus

The system is designed to understand customers beyond simple transactional totals by jointly analyzing:

- Spending levels and monthly expenditure patterns  
- Digital payment usage such as POS, USSD, transfers, and mobile money  
- Savings consistency and income stability  
- Category-level expenses including food, rent, utilities, data, and transport  
- Customer sentiment extracted from feedback and complaints  
- Recurrent complaint themes identified through topic modeling  

Rather than predicting a single risk score, the project focuses on **behavioural grouping**, enabling downstream use cases such as customer profiling, product personalization, and proactive risk monitoring.

---

## Data & Features

The dataset combines **structured financial data** with **unstructured text data**. Financial attributes include demographics, income levels, transaction activity, credit score proxies, and savings behaviour. These are complemented by raw customer feedback, from which sentiment scores and latent complaint topics are extracted using NLP techniques.

All features are transformed into machine-readable formats through encoding, normalization, and scaling, allowing them to be merged into a unified analytical space.

---

## Methodology

The workflow follows an end-to-end applied data science pipeline:

- Data cleaning and normalization of financial variables  
- Encoding of categorical payment and lifestyle attributes  
- Text preprocessing including tokenization, lemmatization, and noise removal  
- Sentiment analysis using NLP models  
- Topic modeling to surface dominant complaint themes  
- Dimensionality reduction using PCA and UMAP  
- Unsupervised clustering with K-Means as a baseline, alongside alternative models such as hierarchical clustering, GMMs, and DBSCAN  

High-dimensional one-hot and text-based features introduce sparsity, which naturally affects cluster compactness. This behaviour is treated as a **realistic constraint of real-world financial data**, not a modeling flaw.

---

## Insights

The resulting clusters reflect **behavioural patterns rather than cleanly separable classes**. Customers tend to overlap in spending habits, payment preferences, and sentiment, especially in markets with informal and hybrid financial behaviours.

Key observations include:

- Numeric financial features drive most of the structural separation  
- NLP-derived features significantly improve interpretability and context  
- Lower silhouette scores are expected and acceptable in this domain  
- Clustering is more valuable for **understanding behaviour** than for achieving perfect metrics  

---

## Visualization & Decision Support

Insights from the clustering and NLP analysis are designed to be consumed through **Power BI or Streamlit dashboards**, enabling:

- Customer segment distribution and behavioural summaries  
- Digital payment adoption trends across segments  
- Expenditure, savings, and credit behaviour comparisons  
- Sentiment trends and dominant complaint topics  
- Monitoring of customer movement between segments over time  

These views support early detection of emerging risk patterns and shifts in customer behaviour.

---

## Key Takeaways

- Unsupervised learning is a discovery tool, not a labeling mechanism  
- Real financial data rarely forms “clean” clusters  
- Feature engineering and dimensionality reduction are critical  
- NLP adds significant value in customer risk understanding  
- Explaining results clearly matters more than optimizing metrics  

---

## Tools & Technologies

Python, pandas, NumPy, scikit-learn, spaCy, transformer-based NLP models, Power BI, matplotlib, and seaborn.

---

## Future Improvements

Planned enhancements include temporal behaviour modeling, hybrid clustering pipelines for mixed data types, automated risk signals derived from cluster dynamics, and deployment as an interactive analytics application.

---

## Author

**Akanbi Benjamin**  
Aspiring Data Scientist | Machine Learning Enthusiast  
Learning in public 🚀
