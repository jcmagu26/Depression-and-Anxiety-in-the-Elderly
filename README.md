# 👵 Depression and Anxiety in the Elderly: Logistic Regression Analysis  

This project analyzes an edited subset of the **Second Longitudinal Study of Aging (LSOA II)** dataset, which is representative of the U.S. civilian non-institutionalized population age 70+ as of mid-1995.  

The goal is to determine whether the proportion of elderly people with depression/anxiety is higher when subsetting based on certain variables, with a focus on **vision problems** and **social activity levels**.  

---

## 📂 Dataset  

- **Source**: Second Longitudinal Study of Aging (LSOA II), subset provided in class  
- **Population**: U.S. individuals aged 70+ (mid-1995)  
- **Variables**:  
  - `DeprAnx`: 1 = frequently depressed/anxious, 0 = not  
  - `VisionBad`: 1 = has trouble seeing even with glasses, 0 = not  
  - `SocialEnough`: 1 = present social activities feel like enough, 0 = too little  
  - `Male`: 1 = male, 0 = female  
  - `Age`: in years  
  - `DaysOut`: number of days leaving the house in the past 2 weeks (0–14)  

---

## 🛠️ Methods  

1. **Descriptive Statistics**  
   - Counts and proportions for binary variables  
   - Summary statistics (mean, SD, IQR) for continuous variables  

2. **Unadjusted Models**  
   - Fit separate simple logistic regressions for each predictor  
   - Calculated **odds ratios (ORs)** and **95% confidence intervals (CIs)**  

3. **Adjusted Model**  
   - Fit a multiple logistic regression including all predictors  
   - Verified **LIBS conditions** (Linearity, Independence, Bernoulli, Simple Random Sample)  
   - Calculated adjusted ORs and CIs  

---

## 📊 Results  

- **VisionBad**: OR = 1.81 → Vision-impaired individuals have significantly higher odds of depression/anxiety.  
- **SocialEnough**: OR = 0.46 → Individuals who feel socially active enough have significantly lower odds.  
- **Male**: OR = 0.68 → Males have lower odds compared to females.  
- **Age**: OR = 0.99 → Slightly lower odds with increasing age (small effect).  
- **DaysOut**: OR = 0.93 → More days outside linked to lower odds of depression/anxiety.  

---

## ✅ Key Findings  

- Vision impairment and lack of social engagement are the strongest predictors of depression/anxiety.  
- Females, socially isolated individuals, and those who spend fewer days outside face higher risk.  
- Targeted interventions (e.g., vision care programs, social support networks) may help reduce risk.  

---

## 📷 Visualizations  

- Empirical logit plots for linearity checks  
- Residual plots for model diagnostics  
- Distribution plots for key variables  

---
