# Telecom-Churn Case Study

**Understanding Data
Understanding the business objective and the data**

The dataset contains customer-level information for a span of four consecutive months - June, July, August and September. The months are encoded as 6, 7, 8 and 9, respectively. 

The business objective is to predict the churn in the last (i.e. the ninth) month using the data (features) from the first three months. To do this task well, understanding the typical customer behaviour during churn will be helpful.

**Understanding the Customer Journey:**

Customers don't typically switch providers overnight. They go through a journey with distinct phases:

**The Good Phase (Months 1 & 2):** Customers are happy with the service and use it regularly.

**The Action Phase (Month 3):** Customer satisfaction might decline due to various reasons like competitor offers, service issues, or billing problems. This is the crucial phase for identifying potential churners.

**The Churn Phase (Month 4):** Customers have discontinued using the service and are considered churned.

**Building the Model: Targeting High-Value Customers**

**Identifying High-Value Customers:**

We'll focus on customers who consistently recharge with substantial amounts, typically exceeding the 70th percentile of average recharge amounts in the first two months (good phase). This filters the data down to a manageable size (around 30,000 customers) while prioritizing those most valuable to retain

**Defining Churn:** Customers with no incoming or outgoing calls and no mobile internet usage in the last month (churn phase) are classified as churned.

**Data Preparation:** We'll remove data from the churn month to avoid biases. This allows us to analyze customer behavior in the "good" and "action" phases and predict their churn risk in the near future.

**Modeling for Actionable Insights:**

We'll build two distinct models to achieve our goals:

**Churn Prediction Model:** This model will analyze customer behavior in the first three months and predict the likelihood of churn. Armed with this information, the company can take targeted actions to retain high-value customers at risk of churning. This might involve offering special plans, discounts, or addressing any service concerns they might have.

**Important Feature Identification Model:**  This model goes beyond simple churn prediction. It delves deeper to identify specific factors in customer behavior that strongly correlate with churn. This allows the company to understand why customers are switching and what aspects of their service need improvement. For instance, the model might reveal a correlation between low call volumes and churn, indicating a need to improve network coverage or offer competitive calling plans.

**Addressing Class Imbalance:**

Since churn rates are typically low (around 5-10%), our data will have a class imbalance. This means there are significantly more non-churned customers compared to churned ones. To ensure the model's accuracy, we'll employ techniques to handle this imbalance, ensuring it doesn't favor the more prevalent (non-churned) class.

**The Benefits: Retention and Growth**

By analyzing customer behavior and building churn prediction models, telecom companies can gain a significant advantage. They can:

**Proactively retain high-value customers:** By identifying churn risk early, companies can take targeted actions to prevent valuable customers from leaving.

**Reduce customer churn:** Lower churn rates translate to increased customer lifetime value and overall revenue growth.

**Gain customer insights:** The churn identification model helps pinpoint the reasons behind customer churn. This allows companies to address service issues, improve offerings, and stay competitive in the market.

In conclusion, churn prediction models are powerful tools that leverage customer data to predict churn risk and identify its root causes. By implementing these models, telecom companies can gain valuable insights into customer behavior, take proactive steps to retain their most valuable customers, and ultimately achieve sustainable growth.
