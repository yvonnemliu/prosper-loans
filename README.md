# Loan Data from Prosper Exploration
## by Yvonne liu


## Dataset

> This data set contains 113,937 loans with 81 variables on each loan. The variables are a good mix of quantitative variables (e.g. BorrowerAPR, ProsperRating, and LoanOriginalAmount) and categorical variables (e.g. EmploymentStatus, Occupation, and Category Listing).


## Summary of Findings

> In the exploration, we found that there was a strong relationship between Borrower APR and Prosper Rating. When Prosper Rating increases, we tend to see a lower Borrower APR.
> However, individual borrowers do not have easy access to their Prosper Rating (an internal rating that Prosper assigns to borrowers). Are there any other factors that borrowers can easily monitor on their end that may have a good correlation with Borrower APR? The answer is yes. We observed a moderate negative correlation between:
>>  1) Borrower APR vs. average credit score. The negative relationship is particularly strong when the Employment Status is Employed, Full-time, Part-time, or Retired (based on our heatmap analysis in the Multivariate Exploration section).
>>  2) Borrower APR and average bank card credit. Borrower APR decreases when the average bank card credit increases.
> We also explored other variables like Employment Status, IsBorrowerHomeowner, and Loan Term to see if they affect the relationship between Borrower APR and Prosper Rating and found some interesting insights:
>> For B-A borrowers, part-time workers usually have the cheapest APR, followed by retired.
>> Whether the borrower is a homeowner or not does not make a difference in APR under each Prosper Rating group.
>> For high-rating borrowers (A or AA), 60-month loans usually have a higher Borrower APR vs. 12-month loans. This makes sense because the more money you want to borrow, the riskier the transaction is for Prosper and the higher your APR is likely to be.

The following analysis is not included in the presentation because it's not related to borrower APR closely.
Out of curiosity, we also explored which occupation has the highest default or past due rate and if that "bad debt" rate is correlated with that occupation's mean income. Our assumption was that the higher the mean income of an occupation, the less likely the loans are past due or charged off or defaulted. We found out that:
> Top three occupations with the highest bad debt rate: all Students!
> Top three occupations with the lowest bad debt rate: Attorney, Landscaping, and Military Officer.
> The higher the montly income of an occupation, the lower the bad debt percentage is likely to be.

## Key Insights for Presentation

> For the presentation, I started by introducing the Borrower APR variable and summarized that the peak frequency occurred around an APR of ~0.35, followed by ~0.30,
We rarely see any APR falling below 0.05 or exceeding 0.40. After that, I plotted the pattern in Prosper Rating (Alpha) distribution and observed that a Prosper Rating of C is the most common Rating type in the dataset, whereas AA is the least common type. 
> Afterwards, I started exploring the variables that have moderate or strong correlation with Borrower APR through a variety of plot types (ie. scatter, heat map, box plot, violin plot, and pointplot). I found that Borrower APR had the strongest relationship with Prosper Rating; however, because individual borrowers' limited access to their Prosper Rating, I also showcased the moderate relationship between Borrower APR and two other variables -- average bank card credit and average credit score -- which are easier to monitor and gain access to for individual borrowers. 
> Next, I introduced more factors into the analysis to evaluate the impact of Employment status, homeownership, loan term, and occupation's mean income on the relationship between Borrower APR and Prosper Rating by leveraging point plot, bar plot, as well as heat maps. The findings vary by the specific Prosper Rating group we are looking at. For example, for AA or HR rating borrowers, we did not see Borrower APR varying by different employment status. This makes sense because their Prosper Rating already speak thousand words about the Borrower APR level they should receive; however, for B-A borrowers, part-time workers usually have the cheapest APR, followed by retired. More findings are summarized in the slide show. 
