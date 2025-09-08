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









<p align="center">
  <img src="6 Assets/Banner.png" width="100%">
</p>

# 🎬 Data-Driven Film Selection and ROI Strategy

*A predictive modeling and business rule framework to help levelFILM pick movies with the highest ROI using internal and external data.*

- Dataset timing: **2000 January – 2023 December**
- Topics covered: **Film Analytics, ROI Modeling, Strategic Timing**
- Models used: **Random Forest, Linear Regression**
- Skills demonstrated: **Data cleaning, model training, business rule design, dashboarding**
- Expected outcome:
    - **Predict ROI and Revenue of films**  
    - **Develop a model-driven acquisition strategy**

---

## 👥 Authors
**Sam Hossain** and MMA Team Gordon Members (Alisha Sahota, Anthony Ramelo, Chris Wu, Elizabeth Zhang, Emily Zhao)

---

## 🔍 Problem Statement

**Goal:**  
Build an end-to-end pipeline to help levelFILM maximize ROI from new film acquisitions by developing predictive models and incorporating them into a strategic dashboard.

**Challenges Addressed:**
- Inconsistent internal and external film data
- Lack of clear acquisition criteria
- Genre and budget bias in historical portfolio
- Unstructured decision-making on release timing
- Need to integrate qualitative rules with predictive scores

This project introduces a comprehensive decision-support framework combining historical performance data with genre, budget, timing, and talent features. It evaluates both revenue and ROI as targets using Random Forest and Linear Regression models, and recommends actionable business rules. Results are delivered through a front-end dashboard where users can test new titles and receive instant ROI predictions.

---

## 🔧 Workflow

### ✅ Data Preparation
- Integrated internal levelFILM acquisition history with external IMDb metadata
- Cleaned, winsorized, and standardized the dataset
- Created derived features: talent points, seasonal indicators, genre dummies, etc.
- Applied correlation filtering and VIF thresholding to reduce multicollinearity
- Engineered final modeling set with 25+ relevant predictors

<p align="center">
  <img src="6 Assets/Data1.png" width="80%">
</p>

### 🤖 Models Built
| Model | Type | Target | Highlights |
|-------|------|--------|------------|
| Model 1 | Linear Regression | ROI | Baseline linear interpretation |
| Model 2 | Random Forest | ROI | Best performing model (R² ≈ 0.66) |
| Model 3 | Linear Regression | Revenue | Basic revenue modeling |
| Model 4 | Random Forest | Revenue | Best for high variance prediction (R² ≈ 0.73) |

**Model Verdict:** Random Forest models outperformed linear models significantly in both ROI and Revenue predictions, capturing nonlinear interactions in budget, timing, and talent.


### 🎬 Acquisition Strategy Design
- Developed business rules from model insights:
  - Target Micro and Indie budget ranges (< $20M)
  - Focus on high-performing genres (Horror, Documentary)
  - Prioritize Canada Day, Christmas, Summer release windows
  - Favor films with strong actor/director scores
- Created an interactive ROI prediction dashboard
- Designed a film scoring method to compare incoming titles
- Recommended A/B testing, quarterly ROI reviews, and continuous model learning

---

## 🎯 Key Findings

* Budget range is the most important ROI predictor (nonlinear effect)
* Genre, timing, and talent play significant roles in ROI variability
* Hindi and German language films showed high ROI outperformance

<p align="center">
  <img src="6 Assets/Findings1.png" width="80%">
  <img src="6 Assets/Findings2.png" width="80%">
  <img src="6 Assets/Findings3.png" width="80%">
</p>

---

## 💡 Key Recommendations

* Implement dashboard to score new titles in real time
* Diversify genre portfolio and set budget thresholds (< $20M)
* Align seasonal release windows with genre trends

<p align="center">
  <img src="6 Assets/Recommendation1.png" width="80%">
  <img src="6 Assets/Recommendation2.png" width="80%">
  <img src="6 Assets/Recommendation3.png" width="80%">
</p>

---

## 📊 Output Dashboard

<p align="center">
  <img src="6 Assets/Dashboard1.png" width="80%">
  <img src="6 Assets/Dashboard2.png" width="80%">
</p>

---

## 🚀 How to Run This Project

1. **Clone the repository**

   ```bash
   git clone https://github.com/SamHossain2025/Film-ROI-Analysis.git
   cd Film-ROI-Analysis
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Launch the dashboard (Streamlit)**

   ```bash
   streamlit run app.py
   ```

4. **Interact with the dashboard**
   - Input film features (budget, genre, talent, etc.)
   - View predicted ROI instantly

---

## 🧬 Data Sources

* 📌 Internal proprietary dataset (anonymized for this project)
* 📌 [IMDb Top 1000 Metadata](https://www.kaggle.com/datasets/harshitshankhdhar/imdb-dataset-of-top-1000-movies-and-tv-shows)

---

## 🔓 License
This project is licensed under the [MIT License](LICENSE)

