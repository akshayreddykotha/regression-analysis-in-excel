# Regression analysis in excel
This analysis has a small dataset which explores the dataset from understanding-the-concept point of view. 

Note:
* Microsoft Excel's regression limits to linear regression analysis however one can try to fit with one independent variable or multiple independent variables.
* R2 is *R-squared value* which is defined as the measure of proprortion of variance of dependent variable explained by the independent variable. The higher the proportion, the better is the relationship between dependent and independent variable/s.

## Dataset 1 - Transit Demand:
The first dataset is a transit demand data set and the dependent variable under consideration is **Number of weekly riders** and there are four independent variables whose predictability we want to know.

**What do the trends say?**

All the scatter plots helps use decide to go for a linear regression model

**What are the assumptions to take care of before applying linear regression model?**
1. There must be a linear relation between independent and dependent variables. 
2. There should not be any outliers present. 
3. No heteroscedasticity 
4. Sample observations should be independent.
5. Absence of multicollinearity and auto-correlation.

The first and second assumptions are met from the above plots. Though it is not an exact linear relation, the whole purpose of modelling is to understand the uncertainty complemented with statistical analysis. Let's apply the regression technique and discover if the assumptions get validated without which our model doesn't stand a suitable fit for the given data and future predictions.

**Evaluation of fit/ model:**

**R2 Value** = 0.95

While R2 is one parameter to look out for the most standard way is to check the residual plots. The more random the errors are, the better your model. It means you shouldn't be able to form a pattern in any part of the plot as far residuals are concerned.

Residual plot for this model:


It can be seen that for fitted values < 140000 of the **Number of weekly riders** variable, residuals are -ve while they are +ve in between [1400000, 150000]. This made me easy to find out which is not the desired outcome.

It's time to evaluate assumptions to check the goodness of fit and find problems with the model in spite of a great R2 value



