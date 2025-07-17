# crime-analysis-stats-project

# Crime Rate Analysis Using Multiple Linear Regression & Hypothesis Testing

This project investigates how law enforcement factors and socioeconomic indicators influence crime rates using **multiple linear regression** and **hypothesis testing**, conducted entirely in **Excel**.

---

## Author
- Janwi Bhattar

---

## 🎯 Objective
To analyze the statistical relationship between crime rates and various factors such as:
- Probability of arrest
- Probability of conviction
- Prison sentencing probability
- Sentence length
- Police per capita
- Population density
- Tax revenue per capita

---

## ❓ Key Questions Explored
- Does the probability of arrest significantly reduce crime?
- Is there a measurable effect of conviction probability on crime rates?
- What is the role of sentencing in crime deterrence?
- Do socioeconomic factors (e.g., tax revenue, population density) impact crime?

---

## 📁 Dataset
- **Source**: FBI Uniform Crime Report (UCR)
- **Sample Size**: 250 rows
- **Dependent Variable**: Crime Rate
- **Independent Variables**:
  - Probability of arrest
  - Probability of conviction
  - Prison sentence probability
  - Police per capita
  - Sentence length (days)
  - Population density
  - Tax revenue per capita

---

## 🔍 Methodology

### 1. Exploratory Data Analysis (EDA)
- Summary statistics and visual inspection using Excel

### 2. Multiple Linear Regression
- Conducted in Excel using `LINEST()` and regression toolpak
- **R² ≈ 0.85**, indicating strong model fit

| Variable                     | Coefficient | P-Value | Interpretation |
|-----------------------------|-------------|---------|----------------|
| Probability of Arrest       | -0.0818     | < 0.001 | Strong deterrent |
| Probability of Conviction   | -0.0365     | < 0.001 | Strong deterrent |
| Police Per Capita           | +3.45       |  0.017  | May reflect response to crime, not cause |
| Average Sentence Length     | +0.0024     |  0.012  | Longer sentences not effective deterrent |
| Prison Sentence Probability | +0.0061     |  0.44   | Not significant |
| Population Density          | +0.00065    |  0.14   | Not significant |
| Tax Revenue Per Capita      | +0.0000517  |  0.36   | Not significant |

---

### 3. Hypothesis Testing

#### 📌 T-Test: Crime Rate (2024 vs 2019)
- **H₀**: μ₍₂₀₂₄₎ = μ₍₂₀₁₉₎
- **Result**: p = 0.681 → **Fail to reject H₀**
- **Conclusion**: No significant difference in crime rates

#### 📌 ANOVA: Crime Rate by Region (Central, West, Urban)
- **H₀**: All regional means are equal
- **Result**: p < 0.05 → **Reject H₀**
- **Conclusion**: Regional differences are statistically significant

---

## 📈 Key Findings
- Increasing arrest and conviction probabilities is more effective than longer sentences.
- Sentencing severity does **not** correlate with lower crime rates.
- Socioeconomic indicators showed **no significant** direct effect in this model.
- Regional variations in crime rates are **statistically significant**.

---

## 📂 Files Included
- `stats_project.pdf` – Full written report
- `regression_model.xlsx` – Excel regression sheet
- `hypothesis_tests.xlsx` – T-test and ANOVA
- (Optional) `crime_data.xlsx` – Raw data (if allowed to publish)

---

## ✅ Conclusion
This Excel-based project demonstrates that **certainty of punishment** is a more effective deterrent to crime than its severity, highlighting a need to focus on **law enforcement efficacy** rather than punishment harshness.

---

