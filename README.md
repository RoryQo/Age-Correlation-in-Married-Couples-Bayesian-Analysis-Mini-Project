# Ages-in-Marriage-Lab-Bayesian-Analysis
Using age data from 100 sampled U.S. married couples, hypothesize a semiconjugate prior, generate a predictive data set to confirm the hypothesis, and use Markov Chain Monte Carlo (MCMC) approximation for mean ages and correlation coefficient.

#### Results
The limited sample size and lack of prior information about the variables in question populations lead to a relatively wide confidence interval using standard frequentist approaches.  Using the Bayesian approach, the confidence interval for the average age of husbands and wives was reduced by over a year.  The confidence interval for the correlation coefficient was reduced by 2% compared to the frequentist.   

After visualizing the relationship, we formed priors for the two variables we are interested in predicting.  Correlation is two-dimensional, so we formulated it following an inverse Wishart distribution, and the mean age for spouses follows a multivariate normal distribution.

Once we establish our priors, we can generate more data by taking random samples of these distributions.  We confirm our priors and data validity by comparing simulated data scatter plots to the actual data scatter plots.  A moderately strong positive correlation is held for each predictive data set relative to the original.

After confirming distributions, we use MCMC approximation to estimate the mean correlation between the age of the husband and the age of the wife.  With the prior information about the data distribution, we can create new confidence intervals for average ages and correlations.

#### Data
The data sampled the age of spouses in 100 sampled U.S. married couples
+ `ageh:` age of husband
+ `agew"` age of wife
