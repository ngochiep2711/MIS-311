# 📘 MIS 311 – Data Analysis and Insights

## 1. Data Overview
The dataset **“Life Expectancy”** contains information on key health and demographic indicators across **182 countries**.  
It focuses on mortality and survival statistics — useful for analyzing the relationship between early-age mortality and average life expectancy.

**Variables included:**
- **Country:** Name of each country (e.g., Japan, France, Nigeria, Brazil)  
- **Region:** Geographical area (e.g., Asia, Europe, Africa)  
- **Infant_deaths:** Number of infant deaths per 1,000 live births  
- **Under_five_deaths:** Deaths of children under five per 1,000 live births  
- **Adult_mortality:** Adult mortality rate per 1,000 population  
- **Life_expectancy:** Average years a newborn is expected to live  

Although the dataset source isn’t explicitly listed, it likely originates from international databases such as **WHO**, **World Bank**, or **UNDP**, which regularly publish mortality and life expectancy statistics.

---

## 2. Data Cleaning Process

### a. Handling Missing Values
Three missing values were found:
- 1 in **Under_five_deaths**
- 2 in **Adult_mortality**
- Countries affected: *Bangladesh, Ghana, and Iraq*

A **Pivot Table** named *“Regional Average of Mortality”* was created to calculate the **average mortality rate per region**.  
Each missing value was replaced by its region’s average — maintaining data consistency and reflecting realistic conditions.

### b. Removing Duplicates
Using Excel’s **Remove Duplicates** function, three duplicate rows were found and removed.  
This ensured each country appeared only once and maintained dataset accuracy.  
A final check with **COUNTBLANK** confirmed there were no remaining missing values.

---

## c. Descriptive Statistics
Descriptive statistics were generated using Excel’s **Data Analysis ToolPak** for four main variables:
- Infant_deaths  
- Under_five_deaths  
- Adult_mortality  
- Life_expectancy  

**Key results:**
- Mean Adult_mortality: **192.15**
- Mean Infant_deaths: **30.36**
- Mean Under_five_deaths: **42.83**
- Mean Life_expectancy: **68.86 years**

➡️ There is **significant variation** in mortality and life expectancy across regions.  
Higher adult mortality contributes strongly to overall lifespan differences, while the wide life expectancy range (**36.85 years**) shows global inequality in healthcare access.

---

## 💡 Insight 1: Adult Mortality vs Life Expectancy
A **scatter plot** was created to visualize the relationship between **Adult_mortality** and **Life_expectancy**.

![Scatter Plot: Adult Mortality vs Life Expectancy](chart1.png)

The graph shows a **negative correlation** — countries with higher adult mortality rates have lower life expectancy.

**Interpretation:**
- Strong healthcare systems → lower adult mortality → longer lifespan  
- Limited healthcare → higher mortality → shorter lifespan  

This highlights the importance of improving adult healthcare, disease prevention, and medical accessibility to raise global life expectancy.

---

## 💡 Insight 2: Infant Deaths vs Under-Five Deaths by Region
A **Pivot Table** and **Column Chart** were used to explore this relationship.

![Column Chart: Infant vs Under-Five Deaths by Region](chart2.png)

The analysis shows a **positive relationship** between the two variables — regions with higher infant mortality also have higher under-five mortality.

**Regional trends:**
- **Africa:** Highest death rates  
- **South America & parts of Asia:** Moderate  
- **Europe & North America:** Lowest rates  

This suggests that **child mortality strongly reflects healthcare development**.  
Regions with better medical infrastructure, nutrition, and vaccination programs achieve lower mortality rates.
