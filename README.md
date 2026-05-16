# • SQL Insurance Claims Analysis  
### Business-Oriented Data Analysis Using PostgreSQL

---

## Project Overview

This project demonstrates SQL-based data analysis using a simulated insurance claims dataset.

It focuses on extracting business insights from structured claims data using PostgreSQL, with an emphasis on identifying patterns in cost, frequency, and claim categories.

The goal is to simulate how data is used in real insurance operations to support decision-making and risk analysis.

---

## Business Context

Insurance companies rely on claims data to understand operational and financial risk patterns.

This type of analysis is used to identify:
- High-cost claim categories  
- Frequent claim types  
- Severity and risk distribution  
- Operational trends in claims processing  

This project simulates that analytical process using SQL.

---

## Analysis Focus Areas

In this project, SQL was used to explore:

- Claim category distribution  
- Total cost per claim type  
- Frequency of claims across categories  
- Aggregated financial impact of claims  
- Pattern identification in structured insurance data  

---

## Analytical Approach

The analysis followed a structured workflow:

**Raw Data → SQL Querying → Aggregation → Business Insight**

The focus was not only on writing SQL queries, but also on understanding what the data represents in a business environment.

---

## Tools Used

- PostgreSQL  
- SQL (Data Analysis & Aggregation)  
- Git & GitHub Version Control  

---

## Example SQL Query (Business Insight)

```sql
SELECT 
    claim_category,
    COUNT(*) AS total_claims,
    SUM(claim_amount) AS total_cost
FROM claims
GROUP BY claim_category
ORDER BY total_cost DESC;
