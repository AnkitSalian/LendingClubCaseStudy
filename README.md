# Lending Club Case Study
> Company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. 
Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'. 
If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.
In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.  The company can utilise this knowledge for its portfolio and risk assessment


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Determine driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.
- Background of project:
  - When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:
    - If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
    - If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company
- Business probem trying to solve:
    - Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'. 
    - If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.
    - In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.  The company can utilise this knowledge for its portfolio and risk assessment.
- Dataset that is being used:
  > loan.csv

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Shorter loan tenures have a higher rate of being fully paid off. In contrast, longer loan tenures have a higher rate of being defaulters.
  > The analysis indicates that loans with longer tenures tend to be riskier, as the percentage of defaults increases with extended repayment periods.
- Loan grades A and B have the highest percentile of fully paid loans, indicating lower risk and higher repayment success. As the grades decline from A to G, the number of fully paid loans decreases, while charged-off loans increase, showing higher risk for lower-grade loans (eg. F, G). 
  > Analysis shows that higher-grade loans are more reliable, while lower-grade loans carry greater risk and are more likely to default.
- Loan grades A and B have the highest percentile of fully paid loans, indicating lower risk and higher repayment success. As the grades decline from A to G, the number of fully paid loans decreases, while charged-off loans increase, showing higher risk for lower-grade loans (eg. F, G). 
  > Analysis shows that higher-grade loans are more reliable, while lower-grade loans carry greater risk and are more likely to default.
- Higher sub-grades (A1 to B5) have more fully paid loans, while lower sub-grade (F5, G3, G5) show an increase in charged-off loans. 
  > This pattern indicates that loans with higher sub-grades are generally repaid more successfully, whereas lower sub-grades have a higher risk of default.
- Home ownership is strongly correlated with loan repayment. Others have the highest number of charged-off loans, while homeowners (mortgage and own) and Rent have significantly lower charge-off rates and higher fully paid loan. 
  > This suggests that home ownership has a significant impact on loan repayment behavior. Individuals with "Other" home ownership status are more risky and are more likely to default on their loans.
- Verification status shows a strong correlation with loan repayment outcomes. Non-verified individuals exhibit the highest fully paid loans. In contrast, loans with verified sources have the highest incidence of being charged off. 
  > This suggests that verification status significantly impacts loan outcomes. Individuals who are verified appear to be riskier and more likely to default compared to others.
- Individuals who take loan for wedding, major purchase, credit card or car are most likely to repay the loan. Thus Purpose is strongly related to loan status.
  > Individuals who took loans for small business or education purposes are riskier and more likely to default.
- The heatmap indicates that loans in IA, IN, ME have the highest percentage of being fully paid with zero defaulters, while NV shows the highest charge-off rate.
  > Individuals from IA, IN, and ME are highly likely to repay their loans. However, individuals from NE present a higher risk and are more likely to default.
- Higher annual income is strongly correlated with better loan repayment. Borrowers with incomes between 1M-6M have significantly higher fully paid loan rates. Borrowers with income between 4k-10k and 500k-1M have significantly higher charged-off loans. Income level is a key factor influencing loan repayment behavior.
  > Accepting loans of individuals whose annual income ranges between 4k-10k are more riskier and are likely to be default wheras individuals with annual income above 1M are likely to repay loan.

### Conclusion of Loan Status over Multiple Categories
- Tenure:
    - Grade A, B with shorter tenure of 36 months experienced higher Full Paid loan wheres grade B, C with tenure of 36 months are more likely to charged off
    > With respect to ongoing loan, loan grade B, C, D, E with bigger tenure are riskier and are likely to default since from past records we can see charge off percentage is greater than person who paid loan.
    - Sub-grade A3, A4 with larger tenure of 60 months experienced Fully Paid Loans wheres sub-grade B4 with larger tenure i.e 60 months are more likely to charged off.
    > With respect to ongoing loan, loan grades B3, B5, C1, C2 are more riskier and likely to be default since from past records we can see charge off percentage is greater than person who paid loan.
    - Individuals with 10+ years of experience with shorter tenure are most likely to fully pay the loan, but for longer tenure we charge off rate is more.
    > With respect to ongoing loan, individuals with 10+ years of experience for larger tenure period are more riskier and are most likely to default.
    - Individuals staying in Rent and short loan tenure are most likely to fully pay the loan, but we see similar trend in charged off as well.
    > With respect to ongoing loan, individual with home ownership as Mortgage with longer tenure period and people who are rented with longer tenure period are risky and most likely to be default.
    - Individuals who are not verified but have shorter tenures exhibit a strong tendency to repay their loans and a moderately strong likelihood of experiencing a charge-off.
    > With respect to ongoing loan, individual irrespective of verification category and applied for longer tenure are more riskier and are likely to be default.
    - Individuals who have applied for debt consolidation for shorter tenure exhibit strong trend to repay the loan and a moderately strong likelihood of experiencing a charged-off.
    > With respect to ongoing loan, individual who have applied for credit card, debt consolidation, home improvement, small business and other pupose for larger tenure are more riskier and are likely to be default
    - Individuals earning 50k-100k for a shorter tenure loan are most likely to repay the loan while individuals earning 10k-50k  for a shorter tenure loan are most likely to get charged off.
    > With respect to ongoing loan, individual whose annual income ranges from 10k-50k, 50k-100k and 100k-500k have applied loan for longer tenure are more riskier and are likely to default.

- Grade:
    - Individuals with 10+ years of experience with grade A exhihit strong tendency to repay the loan and moderately strong likelihood to get charged off.
    > With respect to ongoing loan, individuals with 10+ years of experience with loan grade C, E, G are riskier and are likely to default since from past records we can see charge off percentage is greater than person who paid loan.
    - Individuals who stay in Rent and have loan grade B exhihit strong tendency to repay the loan and moderately strong likelihood to get charged off.
    > With respect to ongoing loan, individuals for loan grade B to E for Mortgage and for loan grade C to E for Rented are riskier and are likely to default.
    - Individuals who are not Verified for loan grade A, B shows strong trend to repay the loan. Individual who are not verified and have loan grade B, C are most likely to get charged off.
    > With respect to ongoing loan, individuals for loan grades C, D, E Source verifed and for loan grades C, D, E are riskier and are likely to default.
    - Individuals who have applied for debt consolidation for loan grade A exhibit strong trend to repay the loan and  individuals who have applied for debt consolidation for loan grade C moderately strong likelihood of experiencing a charged-off.
    > With respect to ongoing loan, individuals for loan grade A debt consolidation is highly likely to pay the loan whereas grades C, E, G for debt consolidation are riskier and are likely to default.
    - Individuals earning 50k-100k for loan grade B are most likely to repay the loan while individuals earning 10k-50k for same loan grade B are most likely to get charged off.
    > With respect to ongoing loan, individuals for loan grade B  earning 50k-100k are most likel to repay the loan whereas loan grades C, D, E earning 50k-100k are more riskier and are likely to default.

- Employee Experience:
   - Individuals with over 10 years of experience who own a home with a mortgage show a strong tendency to repay their loans and a strong likelihood of experiencing a charge-off as well.
   > With respect to ongoing loan, individuals with 10+ years of experience and are rented are most riskier and are likely to default and also there is a small possibility of individuals with 10+ years of experience with Mortgage property might get charged off 
    - Individuals who are not verified with 10+ years of experience shows strong trend to repay the loan. Individual who are verified with 10+ years of experience shows strong trend to get charged off.
    > With respect to ongoing loan, individuals with 10+ years of experience and are verified are most riskier and are most likely to be default.
    - Individuals with 10+ years of experience fo debt consolidation loan purpose are most likely to get charge-off also same category shows moderate likelihood of paying off the loan.
    > With respect to ongoing loan, individuals with 10+ years of experience for debt consolidation are riskier and are mosre likelihood to get default.
    - Individuals earning 50k-100k for employees with 10+ years of experience are less likely to repay the loan and strong likelihood of experiencing a charge-off.
    > With respect to ongoing loan, individuals with 10+ years of experience with 50k-100k annual income are riskier and are most likely to get charged off.

- Home Ownership:
   - Individuals who are not verified and Rented show a strong tendency to repay their loans and a strong likelihood of experiencing a charge-off as-well.
   > With respect to ongoing loan, individuals who are Mortgaged, Rented and are verified are riskier and most likely to default.
   - Individuals who have applied for debt consolidation and Rented show a strong tendency to repay their loans and a strong likelihood of experiencing a charge-off as-well.
   > With respect to ongoing loan, individuals who are Rented and took loan for debt consolidation ae more likely to get default whereas individual with Mortgage and took loan for similar purpose has small probability of getting default.
   - Individuals earning 50k-100k rented are likely to repay the loan and a strong likelihood of experiencing a charge-off.
   > With respect to ongoing loan, individuals who are rented and annual salary is in between 10k-50k are riskier and likely to get default.

- Verification Status
    - Individuals who took loan for debt-consolidation and are not verified exhibit stronger trend to repay the loan whereas individual who applied for same purpose and are verified are most likely to be charged off.
    > With respect to ongoing loan, individuals who are verified and appled for debt consolidation are riskier and are likely to get default.
    - Individuals who has annual income ranging 10k-50k not verified and income ranging 50k-100k not verified exhibit stronger trend to repay the loan whereas income range 10k-50k not verified exhibit strong likelihood to get charged off. 
    > With respect to ongoing loan, individuals who are verified and salary ranges are 10k-100k are more riskier and are likely to get default. For source verified individuals whose salary ranges between 10k-50k are also riskier and likely to get default

- Purpose
    - Individuals who took loan for debt-consolidation and are earning between 50k-100k exhibit stronger trend to repay the loan and a strong likelihood of experiencing a charge-off.
    > With respect to ongoing loan, individuals who applied for debt consolidation and annual income ranges between 4k-10k are riskier and are likely to get default.

### Conclusion on Loan Status with Categories and Numerical Column
- Interest Rate
    - Term
        - Loans with a 36-month term generally have lower interest rates than those with a 60-month term. "Charged Off" loans tend to have slightly higher interest rates compared to "Fully Paid" and "Current" loans across both terms, suggesting a potential relationship between higher interest rates and loan default risk.
    - Grade
        - Lower-grade loans (e.g., D, E, F, G) generally have higher interest rates than higher-grade loans (e.g., A, B, C). "Charged Off" loans tend to have slightly higher interest rates across most grades, indicating a possible correlation between higher interest rates and the likelihood of default. The spread of interest rates increases with lower grades, indicating greater variability in rates for riskier loans
    - Employee Experience
        - Interest rates tend to be consistent across different employee experience, with no significant variation based on the duration of employment. "Charged Off" loans have slightly higher interest rates across most employment lengths, suggesting a correlation between higher interest rates and loan default risk. The spread of interest rates is similar across all employment lengths, indicating that employment length does not significantly impact interest rate variability.
    - Home Ownership
        - Interest rates remain consistent across different home ownership types, with no significant variation based on the type of home. "Charged Off" loans generally have slightly higher interest rates across all home ownership categories, indicating a potential link between higher interest rates and loan default risk. The variation in interest rates is similar across all home ownership types, suggesting that home ownership does not notably influence interest rate differences.
    - Verification Status
        - Verification status significantly impacts loan status. Verified loans have a higher proportion of fully paid loans and lower charged-off rates compared to source verified and not verified loans. This suggests a strong correlation between loan verification and repayment behavior. Interest rates also vary across verification statuses, with verified loans generally having lower interest rates
    - Purpose
        - Interest rates vary slightly across different loan purposes. Car loans generally have the lowest interest rates, while home loans tend to have higher interest rates. "Charged Off" loans generally have slightly higher interest rates across all purposes, indicating a potential link between higher interest rates and loan default risk. The variation in interest rates is significant across different purposes, suggesting that purpose does influence interest rate differences.
    - Annual Income Range
        - As annual income increases, interest rates tend to rise, except within the 1M-6M income range. "Charged Off" loans generally carry slightly higher interest rates across all income ranges, suggesting a potential connection between higher interest rates and loan default risk. The variability in interest rates increases with higher annual incomes, indicating greater fluctuation in rates for riskier loans.
    
- Debt to Income Ratio
    - Term
        - Loans with a 36-month term generally have lower Debt-to-Income (DTI) ratio than those with a 60-month term. "Charged Off" loans tend to have slightly higher debt to income ratio compared to "Fully Paid" and "Current" loans across both terms, suggesting a potential relationship between debt to income ratio and loan default risk.
    - Grade
        - DTI ratio distribution is similar across different loan grades for fully paid, charged-off, and current loans. However, lower grades (E, F, G) tend to have a slightly wider DTI range, particularly for charged-off loans, indicating higher variability in DTI for riskier loan grades. This suggests that borrowers with lower grades might have a higher risk of default.
    - Employee Experience
        - DTI ratio distribution is fairly consistent across different employment lengths for fully paid, charged-off, and current loans. There is no clear trend showing that longer or shorter employment length significantly affects the DTI ratio or the likelihood of loan status outcomes. This suggests that employment length may not be a strong predictor of loan performance when segmented by DTI ratio.
    - Home Ownership
        - Individuals who rent or have a mortgage exhibit a wider range of DTI ratios, especially among those who are fully paid or charged off. Borrowers who own their homes or have no listed ownership type generally show more concentrated DTI distributions. This indicates that home ownership status, particularly renting or mortgaging, may contribute to higher variability in DTI ratios and potential risk in loan outcomes.
    - Verification Status
        - Verification status significantly impacts loan status and DTI distribution. Verified loans have the highest proportion of fully paid loans and the higher DTI levels, while not verified loans have the highest charge-off rates and the lowest DTI ratios. This suggests a strong correlation between verification status, DTI, and loan repayment behavior.
    - Purpose
        - For most purposes, loans with a higher DTI ratio are more likely to be charged off or remain current, rather than being fully paid. Debt consolidation and small business loans have a wider DTI range, suggesting higher risk variability.
    - Annual Income Range
        - The relationship between income category and loan status, segmented by DTI ratio, appears to be moderately strong. Higher income categories show a clear trend of lower DTIs and more fully paid loans, while lower-income categories tend to have higher DTIs and a higher proportion of charged-off loans.
    
- Loan Amount
    - Term
        - Loans with a 60-month term generally have higher loan amounts compared to those with a 36-month term. "Charged Off" loans are more common at higher loan amounts, especially in the 60-month term, indicating a potential link between larger loan amounts and increased default risk.
    - Grade
        - Lower-grade loans (e.g., D, E, F, G) generally involve larger loan amounts compared to higher-grade loans (e.g., A, B, C). "Charged Off" loans are more common in the lower grades (E, F, G), and "Current" loans tend to involve larger amounts, especially in lower grades. The variability in loan amounts is greater for lower-grade loans, indicating higher risk and diversity in borrowing behavior.
    - Employee Experience
        - Loan amounts tend to be consistent across different employment lengths, with no significant variation based on the duration of employment. "Charged Off" loans appear in similar proportions across all employment lengths, suggesting that the risk of default is not strongly influenced by employment length. The spread of loan amounts is also similar across all employment lengths, indicating that employment length does not significantly impact the variability in loan amounts.
    - Home Ownership
        - Loan amounts vary based on home ownership type, with those owning or having a mortgage generally taking larger loans. "Charged Off" loans appear consistently across all home ownership categories, indicating that home ownership does not significantly impact the likelihood of default. The spread of loan amounts is relatively consistent across categories, suggesting that home ownership type does not greatly influence the variability in loan amounts.
    - Verification Status
        - Verification status impacts loan amount, but not uniformly. While verified loans show a higher proportion of fully paid loans, they also have a greater proportion of charged-off loans compared to source verified and not verified loans. This suggests that verification alone may not fully predict repayment behavior, and other factors might influence the likelihood of loan default.
    - Purpose
        - For most loan purposes, "Charged Off" loans exhibit a larger spread in loan amounts compared to "Fully Paid" loans, indicating higher variability and risk associated with default. The exception is the "Moving" purpose, where "Charged Off" loans have a smaller spread than "Fully Paid" loans, suggesting more consistent outcomes for this purpose. This relationship suggests that higher variability in loan amounts may correlate with an increased likelihood of loans being charged off.
    - Annual Income Range
        - As annual income increases, loan amounts generally rise, except within the 1M-6M income range, where loan amounts remain consistent. "Charged Off" loans show a similar distribution across income categories, indicating that higher incomes do not necessarily reduce the risk of default. The variability in loan amounts increases with higher annual incomes, suggesting that larger loans come with greater risk and fluctuation in repayment outcomes.
  
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- pandas - version 2.0.3
- numpy - version 1.24.3
- matplotlib - version 3.7.2
- seaborn - version 0.12.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by the Case Study which Upgrad offered
- This project was based on loan data for all loans issued through the time period 2007 t0 2011.


## Contact
Created by [@AnkitSalian] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
