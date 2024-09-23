# Loan Repayment Prediction Data Analytics Project 
## Project Background
This project analyzes a bank’s loan data to predict whether customers will successfully repay their loans. By applying machine learning models and data analytics techniques, the goal is to improve the bank's loan approval process and reduce the risk of default. This analysis provides key insights into factors influencing repayment behavior, helping the bank make informed decisions about which loans to approve, reject, or price with a higher interest rate.

The dataset contains customer demographic information, loan characteristics, employment data, and historical repayment behavior. The focus is on identifying high-risk applicants before loans are issued, allowing the bank to mitigate financial losses and increase profitability.

## Data Structure Overview
The dataset used for this analysis is structured as a single table that includes multiple features relevant to loan repayment prediction:

**TARGET**: Indicates whether a client had difficulties repaying a loan (1 = repayment difficulties). <br/>
**AMT_INCOME_TOTAL**: Total income of the applicant.<br/>
**AMT_CREDIT**: The total credit amount requested.<br/>
**DAYS_EMPLOYED**: Employment duration of the applicant.<br/>
**FLAG_OWN_CAR/REALTY**: Indicates whether the applicant owns a car or realty.<br/>
_Other features like CODE_GENDER, OBS_30_CNT_SOCIAL_CIRCLE, and DAYS_ID_PUBLISH provide further insights into client behaviors and their social environments._

## Executive Summary
**Key Findings:**
1. **Income Gaps**: The analysis identified substantial income disparities among applicants, especially at the high end of the income spectrum. This gap may raise concerns about the **financial stability** and **repayment capacity** of clients. Targeted lending strategies may be needed to address these risks.<br/>
2. **Credit Amount Trends**: Most clients requested loans within a specific range, suggesting that loan amounts could be customized based on borrower demographics and creditworthiness, leading to **optimized lending practices**.<br/>
3. **Social Circle Influence**: Some anomalies were observed in the **social circle** attributes (OBS_30_CNT_SOCIAL_CIRCLE), which require further investigation. The presence or absence of social influences could affect the likelihood of loan repayment, highlighting the need for more personalized financial assessments.<br/>
4. **Demographic Insights**: Gender-specific patterns emerged, with female applicants representing a slightly higher proportion than male applicants. This could suggest that **loan products** might need to be tailored differently to **male and female** borrowers for optimal risk management.<br/>
   
## Insights and Recommendations
**Category 1: Income and Credit Amounts**<br/>
Applicants with higher incomes tend to request loans within a specific range, but there is a significant gap in income distribution. Recommendations include creating tiered lending products based on income brackets and investigating the relationship between high-income earners and loan defaults.<br/>

**Category 2: Social Circle and Loan Repayment**<br/>
Outliers in the social circle data need to be examined to understand whether social influence correlates with financial behaviors. The bank could consider assessing clients' social environments as part of its risk evaluation processes.<br/>

**Category 3: Demographic Trends**<br/>
Gender and employment duration are key factors influencing loan repayment. Most applicants had employment durations of fewer than 5 years and were between 28 to 50 years old. Recommendations include tailoring loan products to suit applicants' life stages and considering employment history more heavily in loan approval criteria.<br/>

**Category 4: Feature Importance in Predictive Models**<br/>
In the classification models used (e.g., **Random Forest, Logistic Regression**), features such as AMT_CREDIT, AMT_ANNUITY, and EXT_SOURCE_3 were highly predictive of repayment difficulties. Using these insights, banks can enhance their predictive models to pre-emptively identify high-risk clients.<br/>

## KNIME Workflow
• The **data cleaning, preprocessing, and modeling** stages were all carried out using KNIME workflows. The workflows used for this project are accessible here: [KNIME Link].<br/>
• **Classification model** used in this project, including Decision Trees, Random Forests, and Logistic Regression, are available here: [Query & Model Link].<br/>

## Recommendations:
• **Income Gap Analysis**: Given the wide variation in income, focus should be placed on analyzing how income levels correlate with default rates. This could lead to dynamic risk-based interest rates.<br/>
• **Social Environment Influence**: Investigate the social dynamics of high-risk applicants. More research into the social circle data could lead to innovative risk mitigation strategies.<br/>
• **Tailored Financial Products**: Loan products could be better aligned with demographic factors like age, gender, and family status to reduce the likelihood of defaults.<br/>
• **Improved Predictive Models**: Utilizing the most important features such as AMT_INCOME_TOTAL and DAYS_EMPLOYED in machine learning models can enhance risk prediction, leading to more informed lending decisions.<br/>
