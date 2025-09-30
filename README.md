# 🚕 Project: Ridesharing Data Statistical Analysis (Zuber)

**Objective**
Analyze taxi and competitor ride data in **Chicago** to understand passenger usage patterns, identify **key neighborhood destination preferences**, and test the **impact of external factors (weather)** on trip duration to inform the launch strategy of the new ridesharing company **Zuber**.

---

**Results**
* **Competitor Analysis:** **Flash Cab** dominates the market, recording the highest number of trips (Nov 15–16, 2017), suggesting they have the largest coverage or passenger base in the market.
* **Destination Preferences:** The **Loop, River North, and Streeterville** are the top three destinations, concentrating the highest average volume of trips. These areas represent central commercial and high-activity zones.
* **Weather Impact (Hypothesis Test):** A Two-Sample Independent T-Test confirmed that the **average trip duration** from the Loop to O'Hare Airport is **significantly longer** on **rainy Saturdays** compared to non-rainy Saturdays.
* **Statistical Confirmation:** The null hypothesis ($H_0$: Averages are equal) was **rejected** due to a very low p-value, confirming that weather conditions directly influence travel time for this critical route.

---

**Tools**
* **Python**
* **Pandas** (Data manipulation and cleaning)
* **Matplotlib** & **Seaborn** (Data visualization, bar charts)
* **SciPy** (`stats.ttest_ind` for statistical analysis)

---

**Skills Learned**
* **Data Preprocessing and Cleaning** (Type conversion, handling invalid records like 0-second trips).
* **Exploratory Data Analysis (EDA)** (Sorting data, calculating descriptive statistics, visualizing market share and destination ranking).
* **Statistical Hypothesis Testing** (Formulating $H_0$ and $H_1$, defining alpha, selecting the appropriate T-test, and interpreting the p-value).
* **Market Segmentation** (Identifying top destinations for strategic focus).

---

**Improvements / Future Work**
* **Demand Forecasting:** Apply Time Series models to the `start_ts` column to predict peak demand periods for Zuber's fleet positioning.
* **Pricing Strategy:** Analyze the correlation between trip duration (impacted by rain) and fare data (if available) to suggest dynamic pricing during adverse weather.
* **Regional Expansion:** Use the top 10 destination data to prioritize Zuber's initial service area coverage.
