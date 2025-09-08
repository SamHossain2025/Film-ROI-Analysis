<p align="center">
  <img src="6 Assets/Banner.png" width="100%">
</p>

# 🎬 Data-Driven Film Acquisition Strategy

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

---

## 🔧 Workflow

### ✅ Data Preparation
- Integrated internal levelFILM acquisition history with external IMDb metadata
- Cleaned, winsorized, and standardized the dataset
- Created derived features: talent points, seasonal indicators, genre dummies, etc.
- Applied correlation filtering and VIF thresholding to reduce multicollinearity
- Engineered final modeling set with 25+ relevant predictors

### 🤖 Models Built
| Model | Type | Target | Highlights |
|-------|------|--------|------------|
| Model 1 | Linear Regression | ROI | Baseline linear interpretation |
| Model 2 | Random Forest | ROI | Best performing model (R² ≈ 0.66) |
| Model 3 | Linear Regression | Revenue | Basic revenue modeling |
| Model 4 | Random Forest | Revenue | Best for high variance prediction (R² ≈ 0.73) |

**Model Verdict:** Random Forest models outperformed linear models significantly in both ROI and Revenue predictions, capturing nonlinear interactions in budget, timing, and talent.

<p align="center">
  <img src="6 Assets/Model1.png" width="80%">
</p>


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
  <img src="6 Assets/Findings4.png" width="80%">
  <img src="6 Assets/Findings5.png" width="80%">
  <img src="6 Assets/Findings6.png" width="80%">
  <img src="6 Assets/Findings7.png" width="80%">
  <img src="6 Assets/Findings8.png" width="80%">
  <img src="6 Assets/Findings9.png" width="80%">
  <img src="6 Assets/Findings10.png" width="80%">
  <img src="6 Assets/Findings11.png" width="80%">
  <img src="6 Assets/Findings12.png" width="80%">
</p>


---

## 💡 Key Recommendations

* Implement dashboard to score new titles in real time
* Diversify genre portfolio and set budget thresholds (< $20M)
* Align seasonal release windows with genre trends

<p align="center">
  <img src="6 Assets/Recommendation1.png" width="80%">
</p>

---

## 📊 Output Dashboard

<p align="center">
  <img src="6 Assets/Dashboard1.png" width="80%">
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

