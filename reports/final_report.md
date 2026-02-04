Forecasting Financial Inclusion in Ethiopia

Week 10 Final Project Report

1. Introduction

Financial inclusion is a key pillar of Ethiopia’s economic transformation agenda, enabling households and businesses to access formal financial services such as savings, payments, and credit. Over the past decade, Ethiopia has undergone significant structural changes in its financial and digital ecosystems, including the expansion of mobile networks, the introduction of mobile money services, and regulatory reforms aimed at increasing competition.

This project analyzes historical trends in financial inclusion in Ethiopia, identifies key drivers influencing account ownership, and explores potential future outcomes under different policy and infrastructure scenarios. The analysis combines structured data enrichment, statistical forecasting, and scenario-based modeling to support evidence-based decision-making.

2. Data Description and Sources (Task 1)
2.1 Dataset Overview

The analysis uses a unified and enriched dataset stored in:

data/processed/ethiopia_fi_unified_data_enriched.csv


The dataset contains 43 records and 34 variables, structured around four main record types:

Observations – quantitative indicators (e.g., account ownership rate, mobile money usage)

Events – key market, policy, and infrastructure milestones

Targets – national policy goals (e.g., NFIS-II targets)

Impact Links – qualitative relationships between enablers and outcomes

2.2 Key Indicators

Major indicators analyzed include:

Account Ownership Rate (%)

Mobile Money Account Rate (%)

4G Population Coverage (%)

P2P Transaction Volumes and Values

Gender gaps in financial access

Digital ID enrollment (Fayda)

2.3 Data Sources

Data was collected and enriched from credible secondary sources, including:

World Bank Global Findex

Ethio Telecom and EthSwitch reports

National Bank of Ethiopia (NBE)

GSMA, ITU, and A4AI reports

Policy documents such as NFIS-II

All records include metadata on source type, confidence level, and collection date to ensure transparency and traceability.

3. Data Processing and Preparation (Task 1)

Raw and enriched data were processed following a reproducible pipeline:

Conversion of date fields to datetime format

Standardization of categorical variables

Validation and coercion of numeric fields

Separation of raw and processed data into dedicated directories

The cleaned dataset was saved to data/processed and used consistently across all subsequent tasks, ensuring a single source of truth.

4. Trend Analysis and Forecasting (Task 2)
4.1 Historical Trends

Historical analysis of account ownership shows a clear upward trajectory:

2014: 22%

2017: 35%

2021: 46%

2024: 49%

Despite this progress, growth has been uneven, with persistent gender and rural-urban disparities.

4.2 Forecasting Methodology

A linear regression time-trend model was applied using year as the explanatory variable and account ownership rate as the target. Given the limited number of historical observations, a simple and interpretable model was selected.

4.3 Forecast Results

The model estimates continued growth in account ownership. For example:

Projected account ownership for 2026: ~63%

This suggests that Ethiopia is on track toward its medium-term financial inclusion targets, though continued policy and infrastructure support will be required.


5. Driver Analysis (Task 3)
5.1 Objective

Task 3 aimed to identify and quantify the relationship between financial inclusion outcomes and key enabling factors.

5.2 Driver Selection

Based on data availability and relevance, the following drivers were analyzed:

4G Population Coverage (%)

Mobile Money Account Rate (%)

The dependent variable was Account Ownership Rate (%).

5.3 Methodology

A multivariate linear regression model was estimated using only years where all drivers and the target variable were jointly observed. Rows with missing values were excluded to ensure statistical validity.

5.4 Results and Interpretation

Regression coefficients indicate that:

Higher mobile money adoption is strongly associated with increased account ownership

Expansion of 4G coverage also contributes positively, enabling access to digital financial services

Due to the small sample size and data gaps, results are indicative rather than causal and should be interpreted cautiously.

6. Scenario Analysis (Task 4)
6.1 Objective

Scenario analysis was conducted to explore how different policy and infrastructure pathways could affect future financial inclusion outcomes.

6.2 Scenarios Defined

Three scenarios were simulated using the driver model:

Baseline – continuation of current trends

Moderate Expansion – incremental improvements in 4G coverage (+10 pp) and mobile money adoption (+5 pp)

Aggressive Digital Push – accelerated expansion (+20 pp 4G, +10 pp mobile money)

6.3 Results

The model predicts progressively higher account ownership rates under more ambitious scenarios, highlighting the importance of coordinated digital infrastructure expansion and mobile money adoption.

6.4 Policy Implications

Infrastructure investments alone are insufficient without strong adoption of digital financial services

Policies encouraging interoperability and affordability can amplify inclusion gains

Gender-focused interventions remain necessary to close persistent gaps

7. Limitations

Limited historical data points restrict model complexity

Missing values reduce the usable sample for multivariate analysis

Linear models assume constant relationships over time

Future work could incorporate panel data, non-linear models, or cross-country comparisons.

8. Conclusion

This project demonstrates that Ethiopia has made substantial progress in expanding financial inclusion, driven largely by digital transformation and mobile money adoption. Forecasts and scenario analysis suggest that continued investments in digital infrastructure, combined with supportive regulatory frameworks, could significantly accelerate inclusion outcomes.

The findings support the strategic direction outlined in national policies such as NFIS-II, while also highlighting areas where targeted interventions are needed to ensure inclusive and equitable access to financial services.

9. References

World Bank Global Findex Database

National Bank of Ethiopia (NBE)

Ethio Telecom and EthSwitch Reports

GSMA Mobile Gender Gap Reports

A4AI and ITU Affordability Indicators