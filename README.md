# Prediction-of-Loan-Payment-ability (Home Credit Default Risk)
## Objective
A home is not only a major investment for the buyers but also a challenging decision for the mortgage loan lenders as it takes decades to pay off. Among such lenders, Home credit aka, Home Credit B.V., an international non-bank financial institution founded in 1997 in the Czech Republic and headquartered in Netherlands, currently operates in 10 countries including USA and focuses on lending home loan primarily to people with little or no credit history which will either not obtain loans or became victims of untrustworthly lenders.  Hence, Home Credit strives to broaden financial inclusion for the unbanked population by providing a positive and safe borrowing experience by the use of a variety of alternative data, including telco and transactional information, to predict their clients' repayment abilities in addition to their credit history. Hence, in this project I am building a robust model to predict the client’s repayment abilities by employing the various features of the client’s such as: employment, financial status, family status, education and many more rather than solely depending on credit histories.

## Who Might Be Benefitted
This model will directly benefit the mortgage loan lenders such as, Quicken Loans, Wells Fargo, JPMorgan Chase and many more. However, all the consumers and realters are indirectly benefitted by this.

## Datasets
In this project, I am using numerous datasets provided by Home Credit Inc.:
1. **Application**: contains various information of the client at the time of mortgage loan application.
2. **Bureau**: contains data concerning client's previous credits from other financial institutions. 
3. **Bureau Balance**: a monthly data about the previous credits of the applicants in bureau. 
4. **Credit Card Balance**: a monthly data about previous credit cards applicants have had with Home Credit. 
5. **Installments Payments**: payment history of the applicants for previous loans at Home Credit. 
6. **POS_CASH_BALANCE**: a monthly data about previous point of sale or cash loans applicants have had with Home Credit. 
7. **Previous application**: previous applications for loans at Home Credit of clients who have loans in the application data.


## Summary

### Key Findings
1. All sources of datasets contributed to the predictive power of the model. 
2. Model performance scores are exceptionally high with three features External Sources 1,2,3; these features are not clearly explained and also contains higher fraction of missing values. Hence, I excluded these features for modelling.  
3. Out of 6 supervised classification models, Light GBM provided the best results, ROC_AUC 0.75.
4. Top factors that affect the loan repayment ability are: Amount_Credit, Amount_Annuity and Installment payment amount.
5. Based on the business perspective, as illustrated below I divided applicants into 10 tier, applicants lying on the last tier can be completely declined and on second tier can be handled manually and all others can be blindly approved.


![Business Perspectives](https://user-images.githubusercontent.com/66859479/121266328-f151be00-c87f-11eb-929e-295abe09502c.png)





## Further Reading
[Full Project Report](https://drive.google.com/file/d/11Zp79zvFdPQdOuRCEarYdd9GLgddAF49/view?usp=sharing)




