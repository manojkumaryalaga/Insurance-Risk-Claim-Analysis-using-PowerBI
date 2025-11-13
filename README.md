# Insurance Claim and Risk Analysis Dashboard (Power BI)

## Overview
This Power BI project analyzes customer demographics, vehicle characteristics, and claim behavior to identify risk patterns and improve decision-making in the insurance sector.  
It highlights how factors like age, education, car use, and household income affect claim frequency and claim amount.

---

## Dataset Description
The dataset contains anonymized records of insurance policyholders, vehicle details, and claim history.

### Key Columns
- ID: Unique policy identifier  
- BirthDate: Customer's birth date  
- Car Color, Make, Model, Year, Use  
- Coverage Zone: Urban classification (Urban, Rural, Highly Urban, etc.)  
- Education, Gender, Marital Status, Parent, Kids Driving  
- Claim Amount, Claim Frequency, Household Income  

Total Records: 37,542  
Total Claim Amount: $187.8 Million  
Average Claim Amount: $5,006  
Claim Frequency Range: 0–5  

---

## Data Model and Measures
Calculated fields and DAX measures:
- Total Policies = COUNT(ID)  
- Total Claim Amount = SUM(Claim Amount)  
- Average Claim Amount = AVERAGE(Claim Amount)  
- Claim Frequency = AVERAGE(Claim Freq)  
- Claims per Zone = SUM(Claim Amount) by Coverage Zone  
- Claims per Car Make = SUM(Claim Amount) by Car Make  

---

## Dashboard Features
- KPI Cards: Total Claim Amount, Average Claim Amount, Claim Frequency, Total Policies  
- Age and Gender Distribution  
- Claim Breakdown by Education, Marital Status, and Parent Status  
- Claim Value by Car Make, Car Use, and Car Year  
- Regional Comparison by Coverage Zone  
- Household Income vs Claim Amount trend visualization  
- Kids Driving impact on Claim Amount  

---

## Insights Discovered
1. General Overview  
   - The company recorded over 37K policies with a total claim value exceeding $187M.  
   - Average household income among claimants is around $110K.  

2. Demographic Patterns  
   - Mid-aged policyholders (35–45) have the highest total claim value, suggesting higher claim risk.  
   - Married customers contribute a large portion of total claims, while single customers show higher frequency per individual.  

3. Educational and Socioeconomic Insights  
   - Policyholders with a Bachelor's degree make up the largest claim share (~42%).  
   - Higher education correlates with higher claim amounts, potentially due to higher-value vehicles and urban residency.  

4. Vehicle Analysis  
   - Ford and Nissan cars show the most frequent claims, followed by Chevrolet.  
   - Private car usage accounts for 80% of total claims, while commercial vehicles show higher claim frequency but lower total count.  
   - Newer vehicles (after 2010) have increasing claim trends, possibly due to premium car value.  

5. Geographic Insights  
   - Urban and Highly Urban zones have nearly 60% of total claim amount — reflecting dense population and higher traffic exposure.  
   - Rural customers show smaller claim amounts but more stable claim frequency.  

6. Behavioral Findings  
   - Parents with kids driving tend to have lower claim amounts on average.  
   - Customers with higher household income are associated with fewer claims but larger amounts when claims occur.  

---

## Tools Used
- Power BI Desktop for data modeling and dashboard design  
- Power Query for data cleaning and transformation  
- DAX for calculated columns and KPIs  
- Excel as the source data file  

---

## Insurance Dashboard 
---
![Insurance Dashboard](./Dashboard%20Screenshot/Screenshot%20(132).png)

---

## Business Value
- Enables risk-based customer segmentation for insurance pricing  
- Improves underwriting decisions using data-backed insights  
- Supports claim forecasting and fraud risk detection  
- Provides data-driven strategies for policyholder retention  

---

## How to Run
1. Open Insurance_Claim_Risk_Analysis.pbix in Power BI Desktop.  
2. Load the dataset or reconnect to your Excel file if needed.  
3. Explore using interactive slicers (e.g., Education, Zone, Car Make).  
4. Publish to Power BI Service for sharing or embedding.  

---

