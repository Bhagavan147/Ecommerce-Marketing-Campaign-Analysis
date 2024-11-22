# Customer Behavior and Marketing Campaign Analysis

This project focuses on analyzing customer data to uncover patterns and relationships that can drive marketing and business strategies. Using exploratory data analysis (EDA) and feature engineering, the project investigates key factors such as customer income, education, spending behaviors, and campaign engagement. Hypothesis testing is employed to explore whether income influences spending, how marital status impacts wine purchases, and whether lower-income customers are more likely to engage with marketing campaigns. The goal is to derive actionable insights that can enhance targeted marketing efforts and improve customer segmentation.

### Marketing Campaign Dataset  

| **Column**            | **Description**                                                                                   |  
|------------------------|---------------------------------------------------------------------------------------------------|  
| **ID**                | Customer's unique identifier.                                                                    |  
| **Year_Birth**        | Customer's birth year.                                                                           |  
| **Education**         | Customer's education level (e.g., Graduation, Master, PhD, 2nd Cycle, Basic).                    |  
| **Marital_Status**    | Customer's marital status.                                                                       |  
| **Income**            | Customer's yearly household income.                                                              |  
| **Kidhome**           | Number of children in the customer's household.                                                  |  
| **Teenhome**          | Number of teenagers in the customer's household.                                                 |  
| **Dt_Customer**       | Date of customer's enrollment with the company.                                                  |  
| **Recency**           | Number of days since the customer's last purchase.                                               |  
| **MntWines**          | Amount spent on wine in the last 2 years.                                                        |  
| **MntFruits**         | Amount spent on fruits in the last 2 years.                                                      |  
| **MntMeatProducts**   | Amount spent on meat in the last 2 years.                                                        |  
| **MntFishProducts**   | Amount spent on fish in the last 2 years.                                                        |  
| **MntSweetProducts**  | Amount spent on sweets in the last 2 years.                                                      |  
| **MntGoldProds**      | Amount spent on gold in the last 2 years.                                                        |  
| **NumDealsPurchases** | Number of purchases made with a discount.                                                        |  
| **NumWebPurchases**   | Number of purchases made through the company's website.                                          |  
| **NumCatalogPurchases** | Number of purchases made using a catalogue.                                                    |  
| **NumStorePurchases** | Number of purchases made directly in stores.                                                     |  
| **NumWebVisitsMonth** | Number of visits to the company's website in the last month.                                     |  
| **AcceptedCmp1**      | 1 if the customer accepted the offer in the 1st campaign, 0 otherwise (Target variable).         |  
| **AcceptedCmp2**      | 1 if the customer accepted the offer in the 2nd campaign, 0 otherwise (Target variable).         |  
| **AcceptedCmp3**      | 1 if the customer accepted the offer in the 3rd campaign, 0 otherwise (Target variable).         |  
| **AcceptedCmp4**      | 1 if the customer accepted the offer in the 4th campaign, 0 otherwise (Target variable).         |  
| **AcceptedCmp5**      | 1 if the customer accepted the offer in the 5th campaign, 0 otherwise (Target variable).         |  
| **Complain**          | 1 if the customer complained in the last 2 years, 0 otherwise.                                   |  
| **Country**           | Customer's location.                                                                             |  

### Tasks Performed

### Steps for Analysis and Hypothesis Testing  

1. **Exploratory Data Analysis (EDA)**:  
   - Perform a detailed analysis of each feature and column to understand the data's structure, distribution, and any anomalies.  
   - Visualize key features using plots like histograms, box plots, and scatter plots to identify trends and outliers.  

2. **Feature Engineering**:  
   - Engineer new features such as income brackets, campaign acceptance flags, and spending categories for deeper insights.  
   - Create a column categorizing individuals as "In Couple" or "Alone" based on marital status.  

3. **Outlier Handling**:  
   - Identify and remove extreme values if they significantly skew analysis results.  

4. **Hypothesis Testing**:  
   - **Income vs. Education**:  
     - Null Hypothesis (H₀): Income is independent of education.  
     - Tested the relationship between income and education using Kruskal Wallis test.  
   - **Income and Spending**:  
     - Null Hypothesis (H₀): Higher income does not influence overall spending.  
     - Evaluated total spending across all categories using spearman correlation .  
   - **Couples and Wine Spending**:  
     - Null Hypothesis (H₀): Couples spend the same amount on wine as individuals living alone.  
     - Compared wine spending between "In Couple" and "Alone" groups using 2 sample t-test.  
   - **Income and Campaign Acceptance**:  
     - Null Hypothesis (H₀): Campaign acceptance is independent of income level.  
     - Segmented customers into income brackets (above and below median) and analyzed campaign acceptance using a chi-square test.  
