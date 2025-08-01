# Yulu Hypothesis Testing: Understanding Demand Drivers for Shared Electric Cycles

## 🚲 Project Overview

Yulu is India’s leading micro-mobility service provider, offering unique vehicles for daily commutes. With a mission to eliminate traffic congestion and promote sustainable travel, Yulu provides a user-friendly mobile app for shared, solo, and eco-friendly commuting.

This project analyzes Yulu’s electric cycle rental data to identify which variables significantly predict demand in the Indian market and how well these variables explain electric cycle usage. The analysis leverages statistical hypothesis testing and exploratory data analysis (EDA) to provide actionable business insights.

---

## 🏆 Business Problem

**Objective:**  
- Identify significant variables that predict the demand for shared electric cycles in India.
- Quantify how well these variables explain demand.
- Provide data-driven recommendations to optimize Yulu’s operations and growth.

---

## 📁 Dataset Description

**Dataset:** [yulu_data.csv](#)

**Columns:**
- `datetime`: Date and time of the record
- `season`: Season (1: spring, 2: summer, 3: fall, 4: winter)
- `holiday`: Whether the day is a holiday (1: Yes, 0: No)
- `workingday`: 1 if the day is a working day, 0 otherwise
- `weather`: Weather situation (1: Clear, 2: Mist, 3: Light Snow/Rain, 4: Heavy Rain/Snow)
- `temp`: Temperature in Celsius
- `atemp`: "Feels like" temperature in Celsius
- `humidity`: Humidity level
- `windspeed`: Wind speed
- `casual`: Count of casual users
- `registered`: Count of registered users
- `count`: Total rental bikes (casual + registered)

---

## 📝 Analysis Approach

### 1. Problem Definition & Exploratory Data Analysis (EDA)
- Define the business problem and objectives
- Examine data structure, types, and missing values
- Convert categorical variables as needed
- Generate statistical summaries

### 2. Univariate Analysis
- Distribution plots for continuous variables (e.g., temp, humidity, count)
- Barplots/countplots for categorical variables (e.g., season, weather, workingday)

### 3. Bivariate Analysis
- Explore relationships between key variables (e.g., workingday vs. count, season vs. count, weather vs. count)
- Visualize and comment on trends, outliers, and correlations

### 4. Hypothesis Testing
- **2-Sample T-Test:**  
  Test if working days affect the number of electric cycles rented
- **ANOVA:**  
  Test if the number of cycles rented differs across seasons and weather conditions
- **Chi-Square Test:**  
  Test if weather is dependent on season

#### Steps for Each Test:
- Formulate null (H0) and alternate (H1) hypotheses
- Check assumptions (normality, equal variance) using visual and statistical methods
- Set significance level (alpha)
- Calculate test statistics and p-values
- Draw conclusions and business inferences

---

## 📈 Key Questions Explored

- Does being a working day impact electric cycle demand?
- Is demand for cycles similar or different across seasons?
- Does weather significantly affect rental counts?
- Are weather and season statistically dependent?

---

## 🔍 Example Insights

- **Working Days:**  
  Rental counts are significantly higher on working days, suggesting commuter-driven demand.
- **Seasonality:**  
  Demand peaks in certain seasons, indicating opportunities for targeted promotions.
- **Weather Impact:**  
  Poor weather conditions reduce rentals, highlighting the need for flexible fleet management.
- **Variable Relationships:**  
  Weather and season are statistically dependent, which can inform demand forecasting models.

---

## 💡 Business Recommendations

- **Target Working Days:**  
  Focus marketing and fleet availability on working days to maximize utilization.
- **Seasonal Promotions:**  
  Launch campaigns during high-demand seasons to boost ridership.
- **Weather-Responsive Operations:**  
  Adjust fleet deployment and maintenance based on weather forecasts.
- **Data-Driven Planning:**  
  Use insights from statistical tests to refine demand prediction and resource allocation.

---

## 🛠️ Technologies Used

- **Python:** Data analysis and preprocessing (Pandas, NumPy, SciPy, Statsmodels)
- **Visualization:** Matplotlib, Seaborn
- **Jupyter Notebook:** For interactive EDA and hypothesis testing

---
