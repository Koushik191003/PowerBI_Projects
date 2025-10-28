# Bank Customer Analysis
## Objective
The main objective of this project is to analyze customer data from the bank, covering details like demographics, account activities, and credit information. This helps in understanding customer behavior, identifying patterns, and supporting strategies to improve customer satisfaction and loyalty.
## Project Highlights
This project focuses on key aspects such as customer engagement, credit card usage, and account activity. These parameters help the bank to identify which customer groups are active, which need more attention, and how overall engagement can be improved.
## Dashboard Visualization
<img width="1161" height="668" alt="DASHBOARD" src="https://github.com/user-attachments/assets/3001d220-bddd-4b84-a61f-775e75cc49c5" />

## Dashboard Insights
### 1. Customer Activity Chart
   This chart represents the proportion of active and inactive customers. It visually highlights how customer engagement levels vary within the bank.
### 2. Monthly Trend Chart
   The trend chart shows how customer behavior changes month by month. It helps in identifying specific months with higher or lower activity or exits, giving insights into seasonal or operational factors.
### 3. Gender Distribution Chart
   This chart illustrates the distribution of customers based on gender. It helps to understand the balance between male and female customers and how their engagement levels differ.
### 4. Credit Score Category Chart
   This visualization represents customers grouped by their credit score levels such as “Good,” “Very Good,” and “Excellent.” It helps the bank identify which credit groups are more likely to remain active or inactive.
### 5. Summary Cards
   The dashboard includes cards that provide a quick overview of total customers, active/inactive members, and credit card users. These cards make it easy to view the bank’s key statistics at a glance.
## DAX Formulas Used
- Max_Credit = MAX(Bank[CreditScore])
- Totalcustomer = COUNT(Bank[CustomerId])
- Active Member = CALCULATE(COUNT(Bank[IsActiveMember]),KEEPFILTERS(Bank[IsActiveMember]=1))
- Inactive Member = CALCULATE(COUNT(Bank[IsActiveMember]),KEEPFILTERS(Bank[IsActiveMember]=0))
- Credit Holder = CALCULATE(COUNT(Bank[HasCrCard]),KEEPFILTERS(Bank[HasCrCard]=1))
- Not Credit Holder = CALCULATE(COUNT(Bank[HasCrCard]),KEEPFILTERS(Bank[HasCrCard]=0))
- Retain Customers = CALCULATE(COUNT(Bank[Exited]),KEEPFILTERS(Bank[Exited]=0))
- Exit Customers = CALCULATE(COUNT(Bank[Exited]),KEEPFILTERS(Bank[Exited]=1))
## Conclusion
The project highlights how visual analytics can help the bank better understand its customers and make data-driven decisions.
To improve business outcomes based on this analysis:
- Increase engagement programs to encourage inactive customers.
- Focus on improving service experience to retain customers with good credit profiles.
- Conduct periodic feedback surveys to identify satisfaction levels and areas needing attention.
- Strengthen personalized offers and communication to build long-term relationships.
#### These improvements will help the bank enhance customer satisfaction, reduce customer exits, and build stronger customer loyalty over time.
