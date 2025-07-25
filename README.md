# scaledux-ai-internship-task
# 🚀 Startup Health Scoring Model – ScaleDux AI Internship Task

This project is submitted as part of the ScaleDux AI Internship assessment. The objective was to evaluate and score 100 startups based on their business potential using key metrics like user traction, market size, burn rate, and funding.

---

## 📊 Dataset Overview

The dataset `Startup_Scoring_Dataset.csv` includes:

- `startup_id`
- `team_experience`
- `market_size_million_usd`
- `monthly_active_users`
- `monthly_burn_rate_inr`
- `funds_raised_inr`
- `valuation_inr`

---

## ⚙️ Methodology

### 🔍 Data Preprocessing
- Checked for missing values (none found)
- Applied Min-Max normalization to all numeric features
- Inverted `monthly_burn_rate_inr` since high burn is unfavorable

### 📐 Feature Weights

| Feature                  | Weight | Reason |
|--------------------------|--------|--------|
| team_experience          | 15%    | Core team quality |
| market_size_million_usd | 20%    | Bigger opportunity |
| monthly_active_users     | 25%    | Reflects real traction |
| monthly_burn_rate_inr    | 10%    | High burn = risk |
| funds_raised_inr         | 15%    | Investor confidence |
| valuation_inr            | 15%    | Market perception |

A composite score (0–100) was calculated using these weights after normalization.

---

## 📈 Visualizations

- **Score Distribution Histogram** – to view overall score spread
- **Bar Chart of Top 10 Startups** – visualizes the highest performers
- **Correlation Heatmap** – shows relationships between features (e.g. funding ↔ valuation)

---

## 🧠 Insights & Interpretation

### ✅ Top Performer – `S006`
- High user traction, strong team, good market and funding balance.

### ❌ Lowest Performer – `S055`
- Low user count, poor funding, and high burn despite potential.

---

## 🧾 Conclusion

We built a startup scoring model using normalized features and weighted metrics like traction, market size, and funding.  
Burn rate was inverted, as higher values indicate poor financial health.  
Top startups showed strong traction and balanced funding; bottom ones lacked user base or burned too much cash.  
Visuals supported insights, and the model proved useful for evaluating startup potential.  
This approach can guide investors or accelerators in early-stage decision-making.

---

## 📁 Files Included
- `Startup_Score_Ranked.csv` – Final processed score + rank
- `Startup_Scoring_Model.ipynb` – Full notebook with code and visualizations
- `README.md` – Summary of method, insights, and outcomes

---

## 🙏 Thank You

Thank you ScaleDux for this opportunity. I thoroughly enjoyed solving this real-world problem using data science techniques.

> Submitted by: **Dolly Pandey**
> ✍️ Note: README formatting and summary supported with help from AI assistant (ChatGPT), based on my original work.
