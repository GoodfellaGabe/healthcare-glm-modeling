# healthcare-glm-modeling
Generalized Linear Model (GLM) analysis using Negative Binomial regression to predict hospitalizations from NHANES health data.

# Predicting Hospitalizations with Generalized Linear Models (GLM)

**Author:** Gabriel Vasquez  
Led a team of 4 researchers in STAT 171 (General Statistical Models) to investigate significant and non-significant predictors of hospitalization rates using CDC health data. Directed project planning by drafting timelines, delegating roles, and supporting teammates as needed. Personally conducted and interpreted all model diagnostics, model selection, exploratory data analysis, and variable selection, ultimately identifying the Negative Binomial model as the best fit for addressing overdispersion in hospitalization counts.

---

## 📌 Project Overview
This project applied **Generalized Linear Models (GLMs)** to predict the number of hospitalizations for individuals using data from the CDC’s National Health and Nutrition Examination Survey (NHANES).  
Our team investigated overdispersion in Poisson regression and demonstrated the suitability of the **Negative Binomial model**.  

The analysis highlights how demographic, health, and lifestyle factors combine to influence hospitalization risk, and it showcases advanced modeling techniques beyond classical linear regression.  

---

## 🎯 Research Question
> *Which demographic, lifestyle, and health factors significantly influence the number of hospitalizations an individual experiences, and how do these effects interact?*

---

## 📊 Dataset
- **Source:** CDC NHANES sample (subset, ~300 observations)  
- **Variables:**  
  - **Demographics:** Age, Gender  
  - **Health/Lifestyle:** BMI, Cholesterol, Diabetes status, Smoking, Physical Activity  
  - **Response:** Number of hospitalizations (count data)  

---

## 🧮 Methodology
1. **Exploratory Data Analysis (EDA)**  
   - Checked response distribution, exposure rates, and predictor relationships.  
   - Identified overdispersion in hospitalization counts (variance > mean).  

2. **Model Building**  
   - **Poisson GLM** as a baseline.  
   - **Negative Binomial GLM** to address overdispersion.  
   - Added **interaction terms** (e.g., Cholesterol × Diabetes, BMI × Gender).  

3. **Diagnostics & Model Validation**  
   - Likelihood Ratio Tests (LRT), AIC, BIC comparisons.  
   - Variance Inflation Factor (VIF) checks for multicollinearity.  
   - Centered predictors to stabilize interpretation of main effects with interactions.  

---

## 🔑 Key Findings
- **Age:** Each additional year increases expected hospitalizations by ~3.1%.  
- **Cholesterol:** Each unit increase raises hospitalizations by ~2%.  
- **BMI:** Each unit increase in BMI raises hospitalizations by ~53% (stronger effect in females).  
- **Smoking:** Smokers had ~50% higher expected hospitalizations than non-smokers.  
- **Diabetes:** Diabetics had ~81% higher expected hospitalizations.  
- **Interactions:** Significant synergy observed between cholesterol and diabetes, and between BMI and gender.  

---

## 📂 Repository Contents
- `GLM_Hospitalizations.Rmd` — R Markdown file with full analysis.  
- `GLM_Hospitalizations.pdf` — Project report.  
- `scripts/` — Supporting R scripts for EDA, GLM fitting, diagnostics.  
- `figures/` — Plots of model residuals, interaction effects, and fitted distributions.  

---

## 🛠️ Tools & Skills Demonstrated
- **Statistical Modeling:** Poisson & Negative Binomial GLMs, overdispersion testing, interaction modeling.  
- **Diagnostics:** Likelihood Ratio Test, AIC/BIC, VIF, centering.  
- **Software:** R (`MASS`, `car`, `ggplot2`), LaTeX/R Markdown.  
- **Collaboration:** Contributed to model building, EDA, variable selection, and final report writing.  

---

## 🎓 Relevance to Graduate Study
This project demonstrates:  
- Ability to apply **advanced regression techniques** to real-world health data.  
- Critical use of **diagnostics** to justify statistical choices.  
- Competence in both **interpretation** (what coefficients mean in context) and **implementation** (R code, model validation).  

Such skills are directly transferable to graduate-level coursework and research in **statistics, data science, and quantitative finance**, where GLMs and distributional modeling play a central role.  

---

## 📎 References
- Hilbe, J. M. (2011). *Negative Binomial Regression*. Cambridge University Press.  
- Agresti, A. (2015). *Foundations of Linear and Generalized Linear Models*. Wiley.  
- R Packages: `MASS`, `car`, `ggplot2`.  'GGally', 'gridExtra', 'tidyverse', 'dplyr', 'corrplot', 'AER', 'ggplot2', 'interactions', 'aod' 

---

