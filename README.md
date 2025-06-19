# Project Title
# COVID-19-Vaccination-Trends-and-Effectiveness
This end-to-end data analytics project explores global COVID-19 vaccination progress using Python, SQL, and Power BI. It aims to uncover trends in vaccine rollout, identify patterns in manufacturer usage, and assess the efficiency and consistency of different countries’ vaccination strategies.

# What's this project about?
This project explores global COVID-19 vaccination trends using Python, SQL, and Power BI. It analyzes vaccination progress by country, identifies the most-used vaccines, and evaluates rollout consistency and effectiveness. The project answers key questions such as: how quickly countries reached 50% full vaccination, which manufacturers dominated, and how vaccination rates varied over time. It uses two datasets—one tracking daily country-level data and another detailing manufacturer-wise distribution. With Python for data cleaning, SQL for deep querying, and Power BI for interactive dashboards, the project provides actionable insights into global vaccine adoption and country-level vaccination performance.

## 📌 Project Objective
To analyze global COVID-19 vaccination data in order to:
- Track daily and cumulative vaccination trends
- Measure time taken to reach key vaccination milestones (like 50% fully vaccinated)
- Compare vaccine manufacturer usage across countries
- Identify countries with stable and consistent rollout patterns

  ## 📁 Datasets Used

1. **`country_vaccinations.csv`**  
   - Source: [Our World in Data](https://ourworldindata.org/covid-vaccinations)  
   - Contains daily vaccination data for each country  
   - Key fields: `date`, `country`, `daily_vaccinations`, `people_vaccinated`, `people_fully_vaccinated`, etc.

2. **`country_vaccinations_by_manufacturer.csv`**  
   - Source: [Our World in Data](https://ourworldindata.org/covid-vaccinations)  
   - Manufacturer-wise vaccine administration data per country  
   - Key fields: `location`, `date`, `vaccine`, `total_vaccinations`

## 🛠️ Tools & Technologies
 1. Python (Jupyter Notebook) : Data cleaning, preprocessing, analysis 
 2. Pandas / Matplotlib / Seaborn : Data transformation and visualization 
 3. SQL (MySQL/PostgreSQL) : Querying, aggregation, filtering
 4. Power BI : Interactive dashboards, KPI visualization
 5. Git & GitHub : Version control and project hosting

## 📊 Project Workflow

### 🔹 **1. Python (Jupyter Notebook)**
Performed the following:
- Cleaned null values, formatted dates, converted columns to proper datatypes
- Created new columns like 7-day rolling average, dose gap
- Calculated key metrics:
  - Time from first dose to 50% fully vaccinated
  - Gap between first and second dose
  - Consistency in daily vaccination using standard deviation
- Visualized trends using line charts and bar plots

### 🔹 **2. SQL**
Conducted query-based analysis to answer:
- Which country used the most vaccines?
- Which countries reached 1 million doses the fastest?
- Top vaccines globally and country-level usage
- Countries that depended heavily on a single manufacturer (>70%)
- Identified countries with low second-dose completion rates

### 🔹 **3. Power BI Dashboard**

Developed a 3-page interactive dashboard:

  **Page 1: Global Vaccination Overview**
  - KPIs: Total Vaccinations, Fully Vaccinated, Countries Covered
  - Donut chart: Vaccine Share by Manufacturer
  - Country-wise comparison

  **Page 2: Vaccination Progress & Trends**
  - Line chart: Daily & 7-day rolling average
  - KPI: Time taken to reach 50% full vaccination
  - Bar chart: First vs Fully Vaccinated
  - Filters: Country & Vaccine

  **Page 3: Manufacturer Insights**
  - Pie chart: Vaccine share globally
  - Stacked column: Vaccine usage by country
  - Map visual: Geographic distribution of selected vaccines
  - KPI: Vaccine Share % with green/yellow/red status

# Key Analysis Focus Areas
📈 **Vaccination Progress Over Time**
      Analyzed daily and cumulative vaccination trends by country
      Used 7-day rolling averages to smooth short-term fluctuations

⏱️ **Rollout Speed & Milestone Tracking**
      Measured how long each country took to reach 50% full vaccination
      Identified first-dose vs. second-dose gaps

📊 **Manufacturer Usage & Distribution**
      Compared global and country-level usage of vaccine manufacturers
      Highlighted countries highly dependent on a single vaccine

📍 **Consistency of Rollout**
      Calculated standard deviation of daily vaccinations
      Flagged countries with stable vs. erratic vaccine delivery

🌍 **Geographic Insights**
      Visualized vaccine coverage and manufacturer presence using maps
      Enabled regional comparison through filters and slicers

🧠 **Advanced SQL & DAX Insights**
      Ranked countries by performance and diversity in vaccine sourcing
      Created dynamic KPIs and color-coded insights for Power BI

## 💡 Key Insights

  - Pfizer/BioNTech was the most administered vaccine globally
  - Some countries relied on a single manufacturer for >80% of doses
  - Countries with lower standard deviation in daily vaccinations had smoother rollout strategies
  - There’s a visible gap between people who received one dose and those fully vaccinated in many regions

## 📌 Challenges Faced

  - Handling missing data and inconsistent column values
  - Aligning two datasets with different structures (by country vs. by manufacturer)
  - Creating dynamic KPIs in Power BI with proper color formatting
  - Designing a user-friendly, slicer-controlled dashboard layout

## 💼 Business Impact
    📈 Improved Decision-Making :	Helped identify countries with effective vaccine strategies for potential replication
    🏭 Manufacturer Strategy : 	Informed policymakers and health orgs about vaccine dependency and diversity
    🌍 Global Health Insights:	Enabled geographic comparison of vaccine adoption and rollout speed
    ⏱️ Operational Efficiency :	Showed delays and milestones, allowing analysis of rollout logistics
    🎯 Targeted Resource Allocation :	Highlighted areas needing booster doses or manufacturer support

## 🔧 Enhancements & Future Scope
    🗃️ Integration with Case/Death Data	 : Add correlation between vaccination rate and case/death reduction
    📊 Dashboard Automation :	Connect Power BI to real-time or scheduled dataset updates
    🧠 Predictive Modeling :	Use ML models to forecast vaccine demand and coverage in future scenarios
    🗺️ Regional/State-Level Insights	: Enhance granularity by analyzing state-wise rollout (if data available)
    🧩 User Access Control :	Implement role-based views for public, healthcare, or policy users

## Dashboards
1. Global Overview: ![Dashboard Preview](https://github.com/Akanksha311/COVID-19-Vaccination-Trends-and-Effectiveness/blob/main/global%20overview.png)
2. Vaccination Progress and Trends: ![Dashboard Preview](https://github.com/Akanksha311/COVID-19-Vaccination-Trends-and-Effectiveness/blob/main/Vaccination%20Progress%20and%20Trends.png)
3. Vaccine Manufacturer Insights: ![Dashboard Preview](https://github.com/Akanksha311/COVID-19-Vaccination-Trends-and-Effectiveness/blob/main/Vaccine%20Manufacturer%20Insights.png)
