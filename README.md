# Which Debts Are Worth the Bank's Effort?
## Description
After a debt has been legally declared "uncollectable" by a bank, the account is considered to be "charged-off." But that doesn't mean the bank simply **walks away** from the debt. They still want to collect some of the money they are owed. In this project, we will look at a situation where a bank assigned delinquent customers to different recovery strategies based on the expected amount the bank believed it would recover from the customer. The goal for the data scientist is to determine in this non-random assignment whether the incremental amount the bank earns exceeded the additional cost of assigning customers to a higher recovery strategy.

Threshold assignments like this also one occur in medicine (above a certain temperature you get medicine), education (above a certain test score students get admitted to a special class), other areas of finance (above a certain wealth customers get different levels of service), and public sector (below a certain income someone is eligible for housing benefits). Regression discontinuity is an intuitive and useful analysis method in any situation of a threshold assignment.
## Contents 
1. **Regression discontinuity: banking recovery:** Load the data.
2. **Graphical exploratory data analysis:** Create a scatter plot of Age vs. Expected Recovery Amount.
3. **Statistical test: age vs. expected recovery amount:** Compute the average age just above and just below the threshold then test if these average ages are different.
4. **Statistical test: sex vs. expected recovery amount:** Compute the chi-square test for Sex versus Recovery Strategy to see if the sex distribution differs across Recovery Strategy.
5. **Exploratory graphical analysis: recovery amount:** Create a scatter plot of Actual Recovery Amount versus Expected Recovery Amount.
6. **Statistical analysis: recovery amount:** Test if the average actual recovery amounts just above and just below the threshold are different.
7. **Regression modeling: no threshold:** Compute a regression model to predict the actual recovery amount (y) using expected recovery amount (x).
8. **Regression modeling: adding true threshold:** Compute a regression model to predict the actual recovery amount using expected recovery amount and the recovery strategy as the indicator.
9. **Regression modeling: adjusting the window:** Perform the same analysis in task 8, but for the range of $950 to $1050.