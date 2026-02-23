# CAPSTONE PROJECT REPORT

# GLOBAL DEVELOPER SALARY BENCHMARKING

Solving Currency Chaos in Global Talent Acquisition\
Recruitment & HR Analytics \| Stack Overflow Survey 2024 \| INR
Normalization Framework

## SUBMITTED TO

Newton School of Technology\
DVA Capstone --- Cohort 2024\
Data & Visual Analytics Program

------------------------------------------------------------------------

## 1. Executive Summary

### Problem

Recruitment teams hiring globally receive salary data in 100+
currencies. This prevents accurate comparisons and slows hiring
decisions.

### Analytical Approach

Used Stack Overflow Developer Survey 2023. Cleaned to 12,377 valid rows.
Converted all salaries to INR using an IFS-based conversion engine in
Google Sheets.

### Key Findings

-   Andorra, Uzbekistan, and Iceland show highest median salaries.
-   Venezuela and Armenia show highest median experience (18 years).
-   Remote roles show salary premiums.
-   Rust and Go command higher salaries than JavaScript.

### Recommendations

-   Build hiring pipelines in Eastern Europe and Latin America.
-   Standardize salary analysis in INR.
-   Prioritize remote-first hiring.
-   Invest in Rust and Go upskilling.

------------------------------------------------------------------------

## 2. Sector & Business Context

Remote work has created a global talent market. However, salary
comparisons across currencies remain difficult and error-prone.

Talent cost represents 60--80% of tech company expenses. Accurate
benchmarking improves hiring ROI.

------------------------------------------------------------------------

## 3. Problem Statement

Recruitment teams lack a unified framework to compare developer salaries
globally due to currency fragmentation.

------------------------------------------------------------------------

## 4. Data Description

Source: Stack Overflow Developer Survey 2023

Dataset size: - Original: 65,437 rows - Cleaned: 12,377 rows

Key columns: - Country - CompTotal - Currency - YearsCodePro -
LanguageHaveWorkedWith - RemoteWork

------------------------------------------------------------------------

## 5. Data Cleaning

Steps:
- Selected 15 relevant columns and removed the remaining columns to reduce noise and improve processing efficiency.
- Removed rows with missing values in critical fields (salary, experience, country, and currency).
- Extracted currency codes from the raw currency field for accurate mapping.
- Converted salaries to INR using an exchange rate lookup table.
- Standardized country names to ensure consistency across the dataset.
- Performed outlier detection using the IQR method; applied capping (winsorization) at the 5th and 95th percentiles to limit the effect of extreme salary values.
- Used median instead of mean for all aggregations to avoid distortion from remaining skew.

------------------------------------------------------------------------

## 6. KPI Framework

Primary KPIs: - Median Salary (INR) - Median Experience (Years) - Talent
ROI proxy - Language salary premium - Remote work premium

Median used instead of mean due to skewed salary distribution.

------------------------------------------------------------------------

## 7. Key Insights

-   Emerging markets provide senior talent at lower cost.
-   Remote work correlates with higher salaries.
-   Rust and Go developers earn more than high-volume language
    developers.
-   INR normalization enables direct salary comparisons.

------------------------------------------------------------------------

## 8. Talent ROI Corridors

High ROI countries:

  Country     Experience   Salary
  ----------- ------------ ----------
  Venezuela   18 yrs       Moderate
  Armenia     18 yrs       Moderate
  Poland      14 yrs       Moderate
  Romania     13 yrs       Moderate
  Colombia    12 yrs       Moderate

------------------------------------------------------------------------

## 9. Dashboard

Dashboard provides:

-   Country salary comparison
-   Experience vs salary visualization
-   Technology salary leaderboard
-   Remote vs in-person salary comparison

------------------------------------------------------------------------

## 10. Recommendations

-   Build hiring pipelines in high ROI regions.
-   Standardize salary conversion in INR.
-   Upskill developers in Rust and Go.
-   Adopt remote-first hiring policy.

------------------------------------------------------------------------

## 11. Impact

Estimated savings: ₹4.15 Cr per 10-person team annually.

------------------------------------------------------------------------

## 12. Limitations

-   Self-reported salary data
-   Static exchange rates
-   No PPP adjustment
-   Sample bias

------------------------------------------------------------------------

## 13. Future Scope

-   PPP-adjusted analysis
-   Multi-year trend analysis
-   Real-time currency API integration

------------------------------------------------------------------------

## 14. Conclusion

This project delivers a standardized INR-based salary benchmarking
framework to support global hiring decisions.

------------------------------------------------------------------------

## D. Contribution Matrix

| Team Member        | Sourcing | Cleaning | KPI & Analysis | Dashboard | Report Writing | PPT | Overall Role       |
|--------------------|:--------:|:--------:|:--------------:|:---------:|:--------------:|:---:|--------------------|
| Dev Jindal         | O        |          | O              |           |                |     | Team Lead          |
| Aabir Sarkar       |          |          |                | O         |                | O   | Dashboard Lead     |
| Piyush             |          |          |                |           | O              | O   | PPT & Quality Lead |
| Pratyush Choukshey |          | O        |                |           |                |     | Strategy Lead      |
| Bhawana            |          |          | O              | O         |                |     | Analysis Lead      |
| Deepak Pandey      |          | O        |                |           |                |     | Data Lead          |

*Declaration: We confirm that the above contribution details are accurate and verifiable through version history and submitted artifacts.*

Team Signature: \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ Group 8 \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
