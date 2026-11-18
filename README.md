# Bollywood Box Office Performance Analysis

**Entertainment Analytics | Multiple Linear Regression | Predictive Modelling**

A statistical analysis project to investigate the factors associated with Bollywood movie box office collections. Examining the influence of movie budgets, release timing, genre and YouTube audience engagement using Exploratory Data Analysis (EDA), correlation analysis and multiple linear regression.

## Project Objectives

- Identify key factors associated with Bollywood box office performance.
- Analyse the relationship between movie budgets and box office collections.
- Evaluate the influence of release timing and movie genres.
- Examine the relationship between YouTube views, likes, dislikes and box office revenue.
- Develop a multiple linear regression model to quantify the contribution of different predictors.
- Translate statistical findings into actionable insights for film production and marketing decisions.

## Tech Stack

`Python` `Pandas` `NumPy` `Statsmodels` `SciPy` `Matplotlib` `Seaborn`

## Dataset Overview

**149 movie observations | 10 variables**

| Variable | Description |
|---|---|
| Movie Name | Film identification |
| Release Date | Movie release date |
| Release Category | Normal / Long Weekend / Festive / Holiday classification |
| Genre | Defined movie genre |
| Budget | Movie production budget |
| Box Office Collection | Movie box office performance |
| YouTube Views | Online trailer/video views |
| YouTube Likes | Audience engagement |
| YouTube Dislikes | Negative audience engagement |

## Analytical Methodology

1. Data loading, inspection and quality assessment.
2. Descriptive statistics and distribution analysis.
3. Skewness, kurtosis and Jarque-Bera normality testing.
4. Correlation matrix to identify relationships between variables.
5. Categorical variable encoding using dummy variables.
6. Multiple linear regression using Ordinary Least Squares (OLS).
7. Statistical significance testing using coefficients, t-statistics and p-values.
8. Model evaluation using R-squared, adjusted R-squared and F-statistic.
9. Multicollinearity inspection through scatterplot matrices.
10. Residual diagnostics using box plots and Q-Q plots.

## Key Results

### 1. Correlation Analysis

| Variable | Correlation with Box Office Collection |
|---|---:|
| YouTube Likes | 0.68 |
| Budget | 0.65 |
| YouTube Dislikes | 0.62 |
| YouTube Views | 0.59 |

**Key observation:** YouTube Likes and movie Budget demonstrate the strongest positive correlations with box office collections among the numerical predictors.

### 2. Multiple Linear Regression

**Model Performance**

| Metric | Result |
|---|---:|
| R-squared | 60.0% |
| Adjusted R-squared | 56.2% |
| F-statistic | 15.58 |
| Prob (F-statistic) | 4.52 × 10⁻²¹ |
| Observations | 149 |

The overall regression model is statistically significant and explains approximately 60% of the observed variation in box office collections.

### 3. Significant Regression Predictors

| Variable | Coefficient | P-value |
|---|---:|---:|
| Budget | +1.5342 | <0.001 |
| YouTube Likes | +0.0047 | <0.001 |
| Action Genre | -54.5427 | 0.006 |

Other predictors, including YouTube Views, YouTube Dislikes and the individual release-date categories, were not statistically significant at the 5% level in the fitted model.

*Genre coefficients are relative to the reference genre category. The model contains duplicate genre labels caused by inconsistent whitespace in the source data.*

## Business Insights

- **Production Budget:** Demonstrates a positive and statistically significant relationship with box office collections. Investment capacity is an important factor in explaining movie performance.
- **Audience Engagement:** YouTube Likes emerge as a significant predictor, suggesting that positive audience engagement may provide useful insights into movie demand.
- **Views vs. Engagement:** Although YouTube Views have a positive correlation with collections, they are not statistically significant after controlling for other variables. This highlights the distinction between audience reach and engagement.
- **Genre Strategy:** The Action genre indicator has a statistically significant negative coefficient relative to the reference genre in this model. Genre-specific performance should be investigated further.
- **Release Timing:** Release-date categories do not show statistically significant independent effects in the fitted model.
- **Strategic Implication:** Film producers and marketers should consider production budgets and audience engagement indicators together when evaluating potential box office performance.

## Use Cases and Advantages

1. Movie budget and YouTube Likes are statistically significant positive predictors of box office collections.
2. Audience engagement provides additional analytical value beyond measuring video views alone.
3. The regression model explains 60% of observed box office variation, demonstrating the usefulness of combining financial, marketing and categorical movie attributes.
4. Statistical modelling can support more informed decisions regarding production investment, audience engagement and movie marketing strategies.

## Limitations & Future Scope

- Standardise categorical labels and remove inconsistent whitespace.
- Investigate multicollinearity among YouTube engagement variables.
- Explore nonlinear relationships and interaction effects.
- Incorporate additional factors such as star cast, director, critic ratings, competition and marketing expenditure.
- Evaluate model performance using train-test splitting, RMSE and MAE.
- Explore advanced models such as Random Forest, Gradient Boosting and regularised regression.
- Examine whether audience engagement metrics provide predictive value before movie release.

## Conclusion

This project applies statistical modelling to understand the business drivers of Bollywood box office performance. By combining production budgets, release characteristics, genre and digital audience engagement, the analysis identifies meaningful relationships between movie attributes and commercial outcomes.

The output shows importance of production investment and audience engagement in explaining box office performance, which supports data analytics as evidence-based decision-making aid in the entertainment industry.

---

**Project Domain:** Entertainment Analytics | Marketing Analytics | Financial Performance Analysis
