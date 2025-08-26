# 🎬 levelFILM ROI Optimization Project

This project was developed as part of the MMA 804 "Leading Change" course at Queen's University. It focuses on building a data-driven film acquisition strategy for **levelFILM Inc.**, an independent Canadian film distributor.

---

## 🧠 Problem Statement

The traditional genre-based acquisition strategy of levelFILM is no longer sustainable due to:
- Industry dominance by Big 5 studios
- High capital requirements
- Volatility in film performance
- Over-reliance on drama and comedy

The goal: **Build a predictive ROI model** and design a **data-informed acquisition framework** using internal and external data.

---

## 📊 Data Sources

- **Internal Dataset**: Historical data on levelFILM acquisitions (genre, budget, talent, performance)
- **External Dataset**: IMDb Top 1000 Movies and TV Shows ([Kaggle](https://www.kaggle.com/datasets/harshitshankhdhar/imdb-dataset-of-top-1000-movies-and-tv-shows))

---

## 🧪 Analytical Workflow

1. **Data Cleaning & Merging**
2. **Feature Engineering**
3. **Modeling ROI and Revenue**
   - Linear Regression
   - Random Forest (best performance: R² ≈ 0.66 for ROI, 0.73 for Revenue)
4. **Feature Importance Analysis**
5. **Dashboard & Portfolio Strategy Recommendations**

---

## 📈 Key Findings

- **Best ROI**: Micro (<$5M) and Indie ($5M–$20M) budget films
- **Genre Insight**: Horror and Documentaries yield high ROI
- **Timing**: Late spring, Canada Day, and Christmas are ideal release periods
- **Talent Matters**: Certain directors and actors consistently lift ROI
- **Niche Markets**: Hindi and German-language films outperform

---

## 🧩 Deliverables

- 📘 [Final Report (PDF)](./levelFILM%20Report%20-%20Team%20Gordon.pdf)
- 🖥️ [Presentation Slides](./levelFILM%20Pitch%20-%20Team%20Gordon.pptx)
- 🧪 [Modeling Notebooks](./3%20Notebooks/)
- 📊 ROI Predictor Dashboard (coming soon)

---

## 📍 Repository Structure

📁 0 Instructions/
📁 1 Internal Dataset/
📁 2 External Dataset/
📁 3 Notebooks/
📁 4 Presentation & Report/
📄 app.py (Streamlit Dashboard)
📄 roi_model.pkl (Trained RF Model)
📄 requirements.txt
📄 README.md


---

## 🚀 Future Work

- Build and deploy the **interactive Streamlit dashboard**
- Implement a **real-time ROI performance tracker**
- Expand the dataset to include streaming signals and audience sentiment
- Apply **portfolio optimization** using mean-variance frameworks

---

## 👥 Team Gordon (MMA 804 - Leading Change)

- Alisha Sahota
- Anthony Ramelo
- Chris Wu
- Elizabeth Zhang
- Emily Zhao
- **Sam Hossain**

---


