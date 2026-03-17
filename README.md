# 💳 LendingTree: Peer-to-Peer Loan Risk & EDA

## 📌 Project Overview

This project simulates a real-world scenario for a FinTech startup looking to disrupt the peer-to-peer lending market. Using a dataset from **LendingTree**, I performed an Exploratory Data Analysis (EDA) to develop a state-of-the-art risk management strategy. The goal was to identify patterns in borrower behavior, income-to-credit correlations, and geographical risk factors to guide lending decisions across the United States.

-----

## 🏗️ Phase 1: Loan Grade Distribution (Scenario 1)

The first step was to analyze the frequency of different loan grades (A through G) assigned by LendingTree. This helps understand the competitor's risk appetite.

  * **Double Encoding:** Created a bar chart using a color gradient (green to red) to represent risk visually.
  * **Annotations:** Added specific notes to highlight the "default drop-off" point below grade D.
  * **Logic:** Applied `sort_index()` to ensure the risk grades were displayed in their logical order (A to G).

#### Visualisation: Loan Grade Frequency

*Insight: B-grade and C-grade loans are the most common, while grades E, F, and G are rare, suggesting a conservative lending threshold for the startup to model.*

-----

## 🔍 Phase 2: Regional Loan Analysis (Scenario 2)

To identify high-opportunity regions, I analyzed the average loan amounts across the top three states (e.g., Alaska, DC, Hawaii) segmented by grade.

  * **Multi-Index Aggregation:** Utilized `groupby` on both State and Grade.
  * **Unstacking:** Used the `unstack()` method to pivot the data into a structure suitable for a grouped bar chart.
  * **Visual Optimization:** Moved the legend outside the chart area to ensure clear readability of the data clusters.

#### Visualisation: State-Level Grade Distribution

*Insight: Regional differences are clear; for example, Hawaii shows a significantly different risk-to-loan-amount profile compared to Alaska.*

-----

## 🏠 Phase 3: Homeownership & Risk Profile (Scenario 3)

In this phase, I explored whether the composition of homeownership (Rent, Mortgage, Own) changes based on the loan's risk grade.

  * **Stacked Bar Charts:** Created a 100% stacked column chart to compare proportions rather than raw counts.
  * **Compositional Analysis:** Identified how much of the total loan volume in each grade comes from specific borrower profiles.

#### Visualisation: Loan Composition by Homeownership

*Insight: The proportion of renters increases significantly as we move toward higher-risk grades (C, D, and E), suggesting homeownership is a strong indicator of financial stability.*

-----

## 📈 Phase 4: Income vs. Credit Limit (Scenario 4)

Finally, I investigated the correlation between a borrower’s annual income and their total credit limit.

  * **Correlation Analysis:** Identified a moderate Pearson correlation of **0.55**.
  * **Quantile Cutoffs:** Used a vertical line (`axvline`) to mark the **95th percentile**, identifying borrowers making above $170,000.
  * **Outlier Handling:** Focused the plot limits to prevent extreme individual outliers from skewing the visual representation of the general population.

#### Visualisation: Annual Income Correlation

*Insight: While income is a predictor, the variance suggests that the startup needs secondary variables (like the grades analyzed in Phase 1) to accurately set credit limits.*

-----

## 🛠️ Technical Competencies

  * **Advanced Visualisation:** `plt.annotate`, `unstack()`, and 100% stacked charts.
  * **Financial Risk Logic:** Understanding credit grades and debt-to-income indicators.
  * **Data Cleaning:** Managing multi-index dataframes and handling missing values (`NaN`) in unstacked data.

-----

## 🎓 Project Credits

This analysis was developed as part of a specialized Deeplearning's Data Analytics course. It focuses on using Exploratory Data Analysis to solve complex business problems in the financial services sector.

### 🔗 Connect with me: [LinkedIn](https://www.google.com/search?q=https://www.linkedin.com/in/ayushi-gajendra/)
