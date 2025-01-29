# Loan-Apporaval-Analysis
                                                                                          
Introduction:
In the financial sector, loan approvals play a pivotal role in ensuring effective credit allocation while managing risks. These decisions require a thorough evaluation of various factors, such as demographic characteristics, income levels, loan amounts, and credit history. However, the complexity of these interrelated factors often poses challenges for decision-makers.
This project aims to analyze a dataset containing information on loan applications to uncover patterns influencing approval outcomes. By exploring key factors like income, credit history, property location, and demographics, we aim to identify the drivers behind loan approval decisions. Furthermore, the project seeks to develop a predictive model that can assist financial institutions in making more data-driven and efficient decisions, ultimately improving the overall loan approval process

Objectives:
1. Missing Values Treatment
    - Investigate the impact of missing values in the dataset and strategies to handle them (e.g., imputation, removal).
2. Demographic Insights
    - Explore how factors like gender, marital status, number of dependents, education, and employment status influence the likelihood of loan approval.
3. Income & Loan Amount Analysis
    -Analyze the impact of applicant and co-applicant income on loan approval.
    - Determine whether the loan amount requested has any correlation with income or loan approval.
4. Credit and Loan Term Insights
    -  Assess the influence of credit history and loan term on loan approval decisions.
5. Property Area Analysis
    -  Understand how the location of the property affects loan approval chances.

Data Exploration:		
- Load and inspect the dataset.
- Dataframe information and dtypes were explored using df.dtypes and df.describe().
- The categorical columns were analyzed and explored using the groupby  method
 
Handling Missing Data:
 - Handling missing values by replacing ‘Nan’ with ‘Unknown’ and ‘0’ and converting the column according to their data types. 
- The values in the Loan_Status column were replaced from 'Y' to 1 and from 'N' to 0.
- Check how missing data handling affects the dataset and model performance.

Demographic Analysis:
- By using barplot explore the relationship between Loan Approval and Gender.
- By using barplot analyze how Marital Status affects Loan Approval Rates.
- By using groupby on the Dependents  and Loan_Status columns, it calculates the count of each group combination and then reshapes the resulting data with unstack().
- By using barplot investigates how Loan Approval rates vary across different Education Backgrounds
- By using barplot assess how Self-Employment status influences Loan Approval outcomes

Income and Loan Amount Analysis:
- Separate boxplots were used to examine the relationship between Applicant Income and Loan_Status, as well as to analyze the impact of Co-Applicant Income on Loan Approval.
- These plots were then combined using subplots for better visualization and understanding
- Correlation between features was explored and visualized as a heatmap using seaborn 
- The groupby method was used to compare the loan amounts requested by various demographic groups, such as Gender, Marital Status, and Education Level


Credit History and Loan Term Analysis:
- Barplot was used to examine the Loan Approval Rates for applicants with different Credit Histories
- Barplot was used to analyze the relationship between Loan_Amount_Term and Loan Approval Rate.
- A pivot table was used to examine how Credit History interacts with Loan Term.

Property Area and Loan Approval:

   -First, groupby  the data by Loan Approval and Property Area, then use a barplot to analyze the distribution of loan approvals across different property areas and check if property area affects the loan amounts requested.
