# Early-Prediction-of-Motor-Insurance-Claim-Costs-Using-FNOL-Data

## Project Background
Guardian Mutual Assurance (GMA), founded in 1998, is a mid-sized UK insurance provider offering life, auto, and home coverage. Known for affordable premiums and fast claims resolution, GMA has built a strong reputation through digital-first customer engagement.

The company holds extensive claims data, yet early-stage prediction of claim costs at First Notification of Loss (FNOL) remains a challenge. Regulatory requirements demand immediate reserve allocation, but limited initial data often leads to inaccurate estimates impacting profitability, solvency, and customer satisfaction.
This project applies structured exploratory analysis and business-focused insights to improve reserve accuracy and operational efficiency, while enhancing stakeholder confidence in GMA’s claims data.

Insights and recommendations are provided on the following key areas:

•	Claims Pattern Analysis: Identification of trends and correlations across accident severity, third-party involvement, vehicle types, and policyholder attributes.

•	Reserve Allocation Benchmarking: Evaluation of current reserving practices and identification of improvement opportunities using historical data.

•	Operational Efficiency: Recommendations to streamline reserve estimation workflows and reduce delays in claims processing.

Power BI dashboard used to report and explore FNOL Claims data can be found here [(https://github.com/priscy03/Early-Prediction-of-Motor-Insurance-Claim-Costs-Using-FNOL-Data/blob/main/FNOL%20Insurance%20Claims.pdf)]

# Data structure & initial checks

Guardian Mutual Assurance database structure as seen below consists of three tables: Claims Table, Policyholder Table, Third Party Involvement Table, with a total row count of 15, 410 records. A description of each table is as follows:

•	Table 1:claims

•	Table 2:policyholders

•	Table 3:third_parties

<img width="907" height="277" alt="image" src="https://github.com/user-attachments/assets/09425668-1b3a-4129-b184-c70180237038" />

# Executive Summary

Overview of Findings

• This insurance claims analysis uncovers key patterns across operational performance, policyholder risk profiles, and fraud/litigation dynamics.

• The results reveal high claim closure rates, moderate reserve accuracy, region and vehicle specific risk concentrations, and notable overlaps between fraud and litigation cases.

• Recommendations focus on improving reserve practices, enhancing early risk identification, and supporting targeted audits to strengthen financial planning and operational decision-making.

The following sections will expand on reserve accuracy, settlement durations, reserve gaps, customer behavior & vehicle risk patterns possible interactions interaction of fraud and litigation.

# Insights Deep Dive

# Operations:

<img width="874" height="205" alt="image" src="https://github.com/user-attachments/assets/aae2055f-0d04-4cff-a7b2-3ce78a1307ac" />

•	Claim Volume: 800 total claims; 95% settled, 5% still open emphasis on strong closure rate.

•	However Reserve Accuracy: 66% average; moderate alignment between estimated and actual payouts; GMA will not always have enough funds available to meet future liabilities due to over-commitment of capital.

•	 Settlement Duration Average of 102 days (over 3month).Customer impact due to slow or incorrect assessments delays settlements, reducing trust and competitive advantage.

<img width="951" height="253" alt="image" src="https://github.com/user-attachments/assets/09029aff-3a6c-4462-a194-c50982263206" />

•	Estimation of Ultimate payouts are mostly accurate with inaccurate estimation (approx.34%) associated with high and medium claim complexities, potentially associated to third party claims.

•	Most claims over the years have been settled predominately between 31-90 days (approx.3months) followed by 91-180 days (appx.6months).Therefore on average 4 claims per policyholder may be settled by GMA within a year through the claim processes. 

<img width="576" height="168" alt="image" src="https://github.com/user-attachments/assets/b6d2daac-2d98-4106-ab6e-3c09790d3293" />

•	The frequency of collision claims is the most over the years, however claim type associated to fire has the largest average absolute reserve gap and would likely cause more reserve accuracy inconsistencies;

•	Insurance Claims associated to fire is difficult due to the complexity of fire and secondary damages (smoke, water (fire fighters), subject to valuation methods, and disputes over documentation and policy terms. 

# Claim Patterns:

<img width="715" height="137" alt="image" src="https://github.com/user-attachments/assets/13c0645d-32a9-4a87-adb6-feddaa5e9eaf" />

•	There are about 5000 policy holders, with an average annual mileage over the years of 12.13 thousand miles.

•	Policy members spanning over 10 regions with approx. £ 99 million in ultimate claims.

•	Third party involved in claims in about 25%, which although not too high is significant enough to impact or influence final claims.


<img width="550" height="189" alt="image" src="https://github.com/user-attachments/assets/4b7ac3bf-9ea7-47c7-82c0-1990caa8f42f" />


•	Top 3 regions in frequency of claims are Glasgow, Liverpool and Bristol, with employed and retired policy holders dominating the claims and unemployed holders with the least ( employed and retired would tend to use vehicles more than unemployed )

•	Sedans have a larger frequency in claims yet coupes have a larger ultimate claim, reflecting volume may not always reflect amount in claims, insurance claims are usually based on the value of the property insured.

•	Policy members with less than 5 years driving experience average claims are the highest .It could be said, a policy member claim from Glasgow or Liverpool , driving a coupe and has less than 5 years driving experience would have a higher claim on average.

<img width="407" height="243" alt="image" src="https://github.com/user-attachments/assets/3b8aad06-0f7e-457e-b87a-a2597ec7ff70" />

•	Policy members with Excellent and Good credit scores tend to have higher average ultimate claims, as there company experience incomplete information at FNOL, credit score can be used as a preliminary indicator of estimated claim.

•	Third party claims are usually of minor severity, thereby from duration would likely not exceed average duration of claim settlement (i.e. 102 days).Further investigation would be required, perhaps into fraud or litigation.

# Fraud and Litigation:

<img width="325" height="324" alt="image" src="https://github.com/user-attachments/assets/de1704b3-2c29-46e2-9902-2482be4104d5" />

•	As the average loss and cost of litigation are so close together, it can be expected that there will be an overlap in fraud and litigation.It could be said most fraud cases could lead to litigation , there by delaying duration of ultimate claims 

# Recommendations:
Based on the insights and findings above, we would recommend the Guardian Mutual Assurance (GMA) to consider the following:

# Claims Pattern Analysis;

Recommendation:

• Develop region- and demographic-specific risk profiles to inform underwriting and pricing strategies.

• Use vehicle type, driving experience, and credit score as early indicators in FNOL triage to guide reserve estimation and claims prioritization.

# Reserve Allocation Benchmarking;

Recommendation:

• Benchmark reserve accuracy by claim type and complexity level to identify underperforming segments.

• Introduce reserve calibration guidelines for high-risk categories (e.g., fire, third-party involvement) based on historical payout patterns.

# Operational Efficiency;

Recommendation:

• Implement fast-track workflows for low-severity and third-party claims to reduce average settlement time.

• Flag potential fraud-litigation overlaps early to allocate appropriate resources and reduce downstream delays.

• Consider a dedicated review process for fire claims to address documentation and valuation challenges.

# Enhanced Recommendation;

Next step; Integrate Machine Learning for predictive claim costing and perhaps potential fraud detection in the long run.

# Assumptions and Caveats:

Assumptions;

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:

•	Claim Closure Equals Settlement: Closed claims were assumed to be fully settled, with no pending adjustments or disputes.
  
•	Credit Score as Proxy for Asset Value: Higher credit scores were interpreted as indicative of higher-value vehicles or assets.

•	Vehicle Type Reflects Claim Cost: It was assumed that vehicle type (e.g., coupe vs. sedan) correlates with repair or replacement cost.

•	Fraud and Litigation Overlap: The observed proximity in cost and regional concentration was treated as indicative of overlap, though causality was not confirmed.

Caveats;

These are limitations or considerations that stakeholders should keep in mind when interpreting your findings:

• Correlation ≠ Causation: While patterns were identified (e.g., younger drivers with higher claims), these do not imply direct causality.

• Reserve Accuracy Benchmarking: The 66% reserve accuracy figure is based on historical payout alignment and may not reflect current actuarial models.

• Regional Risk Profiles: High claim frequency in certain regions may be influenced by population density or policyholder demographics, not necessarily higher risk.

• Fraud Flagging Sensitivity: Fraud detection rates depend on internal flagging criteria, which may vary over time or across teams.

• Litigation Cost Attribution: Costs associated with litigation may include legal fees, delays, and settlements, but were not broken down in this analysis.

•	Historical Scope Only: Analysis relied on past claims data; real-time integration was beyond scope.







