🛒 Customer_Behaviour_Analysis
Data Analysis project showcasing customer behaviour analysis using Python, SQL, and Power BI.

🌟 Overview: This repository contains an end-to-end data analytics project focused on understanding consumer shopping behavior for a leading retail company. The primary objective is to transform raw customer data into actionable business intelligence to optimize marketing strategies, enhance customer engagement, and drive long-term loyalty. The lifecycle of the project spans data engineering in Python, relational database analysis in PostgreSQL, executive dashboard development in Power BI, and AI-assisted stakeholder presentation generation using Gamma. 

📅 Dataset: The analysis is based on a transactional retail dataset capturing customer purchasing attributes. 
    ➡️ Dataset Size: 3,900 rows and 18 columns.  
    ➡️ Missing Data: 37 missing observations isolated within the Review Rating attribute.  
    ➡️ Core Features:
      ✅ Demographics: Age, Gender, Location, and Subscription Status.  
      ✅ Purchase Details: Item Purchased, Category, Purchase Amount (USD), Season, Size, and Color.  
      ✅ Behavioral Metrics: Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, and Shipping Type.  
      
🛠️ Tools & Technologies 
    ➡️ Data Processing & EDA: Python (Pandas, NumPy, Matplotlib, Seaborn)  
    ➡️ Database Management System: PostgreSQL (SQL DDL/DML, Advanced Window Functions, Join Operations)  
    ➡️ Business Intelligence: Power BI Desktop (Data Modeling, Star Schema, UI/UX Design)  
    ➡️ Reporting & Presentation: Gamma AI (Executive Slide Deck Design)  
    ➡️ Version Control: GitHub  

🚀 Execution Steps
1. Data Preparation & Engineering (Python)
   ➡️ Ingestion: Loaded the raw dataset using the Pandas engine for structural inspection.
   ➡️ Exploratory Data Analysis (EDA): Implemented df.info() and df.describe() to capture initial structural summary statistics.
   ➡️ Handling Missing Values: Cleaned data by imputing the 37 null values in the Review Rating column using the median rating of each respective product category.
   ➡️ Standardization: Renamed columns to standardized snake_case format to optimize documentation readability.
   ➡️ Feature Engineering:
       ✅ Binned customer ages to generate a categorical age_group column.
       ✅ Derived a purchase_frequency_days column from temporal data points.
   ➡️ Redundancy Validation: Verified a high correlation between discount_applied and promo_code_used, dropping the redundant promo_code_used feature.
   ➡️ Database Pipeline: Established a secure connection layer to load the fully transformed DataFrame into PostgreSQL.

2. Deep Dive Data Analysis (SQL) Using PostgreSQL, advanced analytical queries were structured around transaction simulations to answer core business metrics:
   ➡️ Demographic Metrics: Segmented total revenue across genders (Male: $157,890 | Female: $75,191) and isolated purchasing patterns across calculated age brackets.
   ➡️ Behavioral Deep Dives: Identified 839 high-spending discount users who beat average purchase values, and cross-referenced purchase histories to group customers into New (83), Returning (701), and Loyal (3,116) cohorts.
   ➡️ Product Insights: Queried the top 5 highest-rated products (led by Gloves at 3.86), calculated the top 3 items per category using RANK(), and discovered discount-dependent items (e.g., Hats have a 50% discount dependency rate).
   ➡️ Operational Performance: Evaluated shipping types, showing that customers utilizing Express Shipping spend a higher average amount ($60.48) than Standard users ($58.46).

3. Business Intelligence Dashboard (Power BI)
   ➡️ Built a high-fidelity, interactive Customer Behavior Dashboard to turn structured SQL outputs into visual narratives.
   ➡️ KPI Trackers: Deployed dynamic cards highlighting 3.9K Total Customers, $59.76 Average Purchase Amount, and 3.75 Average Review Rating.
   ➡️ Cross-Filtering Views: Developed comparative matrices analyzing Subscription Status (73% Non-Subscribers vs. 27% Subscribers), Sales and Revenue by Category (dominated by Clothing), and Age Group distribution.
   ➡️ Slicers Implemented: Interactive filtering by Subscription Status, Gender, Category, and Shipping Type.

4. Stakeholder Presentation (Gamma)
   ➡️ Summarized complex backend analytical data frameworks into an executive markdown project report.
   ➡️ Generated a highly visual slide presentation utilizing Gamma to deliver concise strategic suggestions to non-technical leadership teams.

📊 Dashboard Preview: The interactive Power BI interface is modeled with the following key visual segments:  
    ➡️ Top Metric Ribbon: Instantly displays customer counts, average spending tickets, and customer satisfaction scores.  
    ➡️ Subscription Breakdown: A donut chart isolating subscription adoption across customer categories.  
    ➡️ Categorical Volume Bars: Coupled column charts mapping total order volumes and revenue across key product fields.  
    ➡️ Demographic Matrices: Paired bar charts mapping sales counts and revenue contributions against age brackets.  

✅ Business Recommendations & Results: 
  ➡️ Maximize Subscription Values: Incentivize the 73% non-subscriber base by introducing exclusive member-only loyalty discounts to scale repeat buyer metrics.  
  ➡️ Refine Discount Rules: Optimize product margins by revising policies on discount-dependent products like Hats and Sneakers.  
  ➡️ Targeted Campaign Budgets: Allocate marketing spend heavily towards high-revenue age segments (Young Adults) and express-shipping buyers.  
  ➡️ Strategic Product Positioning: Feature high-volume and top-rated items (Gloves, Sandals, and Clothing) in primary promotional carousels.  
    
