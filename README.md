# Life-Expectancy---Linear-Regression
R project based on the datasaet is "Liffe Expectancy (WHO)" (https://www.kaggle.com/kumarajarshi/life-expectancy-who). 
Moreover, the dataset involved all the countries in the time span 2000-2015 but the analysis focused only on the year 2015. A linear regression was carried out in order to identify
the main factors influencing Life Expectancy. The target is life expectancy and is expressed in years-old. The first task was data preprocessing: 1 - extracting data referred 
to the year 2015; 2 - excluding NA rows; 3 - merging all the vaccine per desease variable in just one variable; 4 - creating a Bernoulli variable for developing and not developing
countries; 5 - correlation matrix in order to identify the most correlated predictors and, in case of high correlation, they are left out. Correlation matrix was useful to detect 
high correlation between the predictors and the target variable, too. In case of high correlation, those variable could be highly informative.
Once completed the pre-processing phase the focus was on the detecting the best model. Starting from a full model, not significative variable have been gradually removed. The 
procedure to identify the best model was based on all subset regression, using BIC. The best model was composed of the variables: Adult.Mortaly, Polio, Schooling and HIV.AIDS.
The model diagnositcs was carried out through the following hypothesis tests: 1 - Test of normality (Shapiro/Wilk test, Kolmogorov/Smirnov test, Anderson/Darling test, Cramer/Von
Mises test, Pearson test, Lilliefors test, Shapiro/Francia test) Normality hypothesis not rejected. Furthermore, normality was also checked through the analysis of residuals; 
2 - Test for homoskedasticity (Breusch/Pagan test); 3 - Test for incorrelation (Durbin/Watson test). The linearity property was checked through partial regression plot.
