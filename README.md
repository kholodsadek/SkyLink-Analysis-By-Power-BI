# SkyLink-Analysis-By-Power-BI
## Project Overview
As a Business Intelligence Analyst at Gulf Researcher, you are tasked with analyzing customer churn rates for SkyLink, a telecommunication company. The project involves investigating a dataset containing detailed customer information to uncover the reasons behind customer churn and provide actionable insights to reduce it. Using Microsoft Power BI, create visually compelling report pages to help SkyLink better understand and manage customer churn. This analysis will focus on identifying key factors driving churn and addressing specific questions posed by SkyLink to enhance customer retention strategies.

## Data Cleaning (Transformation)
- **Churn Category**: Replace blank values with `"No Churning"`.
- **Churn Reason**: Replace blank values with `"No Reason As No Churning"`.
- **New Column**: Create a new column to indicate whether the customer has churned by checking if the churn label is `"Yes"`. This will simplify the calculation of the total number of churned customers.

## Analysis
1. **Current Churn Rate**:
   - Calculate the current churn rate: `((total churned customers / total customers) * 100) = 30.6%`.
   - Visualize this in a pie chart using `CustomerID` and `Churn Label`.
   - ![Current Churn Rate](/images/pie%20chart.PNG)

2. **Churn Categories**:
   - Identify the most prevalent churn category by visualizing it in a bar chart. The category with the highest number of customers is `"Competitor"`.
   - ![Churn Category](/images/Churn%20category.PNG)

3. **Churn Rate by State**:
   - The churn rate varies across different states.
   - The state with the highest churn rate is California (`CA`).
   - ![churn per state](/images/churn%20rate%20per%20state.PNG)

4. **Churn Rate by Age**:
   - The churn rate increases with age.
   - Churn rate for customers under 30: `26.15%`.
   - Churn rate for customers over 65: `43.44%`.
   - The relationship shows that younger customers (`<30`) have a lower churn rate, while older customers (`>65`) have a higher churn rate.
   - ![churn per age](/images/churn%20rate%20per%20age.PNG)

5. **Churn Rate by Group Size**:
   - The group size with the lowest churn rate is `3`, with a churn rate of `5.63%`.
   - ![churn in number of groups](/images/churn%20rate%20per%20number%20in%20group.PNG)

6. **Contract Type and Churn**:
   - Customers with monthly contracts have the highest churn rate.
   - ![churn rate per contract type](/images/churn%20by%20contract%20type.PNG)

7. **Unlimited Data Plan and Churn**:
   - Customers without an unlimited data plan are more likely to churn.
   - The highest churn rate occurs when data consumption reaches `41 GB`.
   - ![churn in unlimited data plan](/images/churn%20rate%20per%20unlimited%20data%20plan.PNG)

8. **International Activity and Churn**:
   - Increased international activity correlates with higher churn rates.
   - ![churn in INtl Active](/images/churn%20per%20Intl%20Active.PNG)

9. **Customer Insights**:
   - **Payment Method**: `"Direct Debit"` is associated with higher churn, while `"Paper Check"` is associated with lower churn.
   - ![churn in payment method](/images/churn%20by%20payment%20method.PNG)
   - **Account Length**: As account length decreases, churn increases.
   - ![churn in Account Length](/images/churn%20by%20account%20length%20.PNG)
   - **Contract Type**: Monthly contracts increase churn, while `"Two Year"` contracts decrease it.
   - ![churn in Contract type](/images/churn%20by%20contract%20type.PNG)
   

## Measures
1. **Churn Rate for Specific Customer Group**:
   - The churn rate for customers not in a group plan, aged 50, with an account length of 12 months or less is `48.57%`.

2. **Customer Service Calls and Churn**:
   - The average number of customer service calls for customers on a monthly contract who pay by direct debit is `1.57`.
   - The churn rate for these customers is `58.47%`.

3. **Extra Data Charges and Churn**:
   - The average extra data charges for customers not on an unlimited data plan and consuming 10 or more GB is `$30.20`.

---
