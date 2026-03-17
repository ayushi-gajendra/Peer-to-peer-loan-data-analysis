# 💳 LendingTree: Peer-to-Peer Loan Risk & EDA

## 📌 Project Overview

This project simulates a real-world scenario for a FinTech startup looking to disrupt the peer-to-peer lending market. Using a dataset from **LendingTree**, I performed an Exploratory Data Analysis (EDA) to develop a state-of-the-art risk management strategy. The goal was to identify patterns in borrower behavior, income-to-credit correlations, and geographical risk factors to guide lending decisions across the United States.

-----

## 🏗️ Phase 1: Income & Credit Limit Correlation

The first step was to determine if a borrower's annual income is a reliable predictor of their total credit limit. This is foundational for setting automated loan approval thresholds.

  * **Statistical Thresholding:** Identified that borrowers with an annual income above **$170,000** represent the top 5% of the dataset.
  * **Outlier Management:** Applied axis limits to focus on the core population (income under $500k) to prevent extreme outliers from skewing the strategy.
  * **Visualization:** A scatter plot with an annotation for the 95th percentile income threshold.

#### Visualisation: Income vs. Credit Limit

*Insight: While a positive correlation exists, the high density of points at lower income levels suggests that income alone cannot be the sole factor for high credit limits.*

-----

## 🔍 Phase 2: Risk Grading & Homeownership

To build a "risk-aware" product, I segmented the data by loan grades (A through G) and homeownership status.

  * **Multi-Dimensional Analysis:** Analyzed how homeownership (Mortgage, Rent, Own) varies across different credit risk grades.
  * **Findings:** Borrowers with mortgages are consistently more prevalent in higher-grade (lower risk) categories, suggesting higher financial stability.

#### Visualisation: Loan Grades & Homeownership

*Insight: High-risk grades (E, F, G) show a higher proportion of renters compared to Grade A, providing a clear signal for the startup's risk model.*

-----

## 🗺️ Phase 3: Regional Risk Analysis

A state-by-state analysis was performed to identify geographical clusters of high-risk or high-opportunity borrowers.

  * **Segmentation:** Grouped data by US State and Loan Grade.
  * **Logic:** Identified specific states where "Grade A" loans are dominant versus states with higher default risks.

#### Visualisation: State-Level Grade Distribution

*Insight: This regional heatmap/bar chart allows the startup to tailor interest rates based on the economic stability of specific geographic zones.*

-----

## 📊 Phase 4: Loan Purpose & Volume

Understanding *why* people borrow is as important as *how much* they borrow. I analyzed loan counts across different categories to identify market demand.

  * **Categorization:** Segmented loans by purpose (Debt Consolidation, Credit Card, Home Improvement, etc.).
  * **Visual Optimization:** Created a refined column chart to highlight the primary drivers of loan applications.

#### Visualisation: Loan Purpose Volume

*Insight: Debt consolidation remains the primary driver of loan requests, suggesting the "disruptor" product should focus on streamlined balance transfer features.*

-----

## 🛠️ Technical Competencies Demonstrated

  * **Advanced Data Visualisation:** Using `plt.annotate`, `axvline`, and custom styling to make charts "boardroom ready."
  * **Risk Segmentation:** Applying financial logic (95th percentile, grading) to raw data.
  * **Data Cleaning & Filtering:** Handling large-scale financial datasets with Python.
  * **Business Storytelling:** Moving from code to strategic recommendations for a hypothetical startup.

-----

## 🧠 Strategic Takeaway

This EDA proves that a successful risk management strategy must be **multidimensional**. By combining income thresholds, homeownership stability, and geographic trends, the startup can minimize defaults while maximizing market share in high-demand categories like debt consolidation.

-----

## 🚀 How to Run

1.  Clone this repository.
2.  Install dependencies: `pip install pandas matplotlib seaborn`.
3.  Open `Lendingtree-Loan-data-analysis.ipynb` and run the cells.

-----

## 🎓 Project Credits

This analysis was developed as part of a Deeplearning Data Analytics course focused on applying **Exploratory Data Analysis** to solve complex business problems in the financial services sector.

### Author

**Ayushi Gajendra**
*Data Analyst | Former EdTech Co-Founder*
[LinkedIn](https://www.google.com/search?q=https://www.linkedin.com/in/ayushi-gajendra/) 

-----

**Next Step:** Would you like me to help you create a **Summary Table** for this README that compares the "Average Interest Rate" across different Loan Grades?
