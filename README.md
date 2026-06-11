# Voter-Turnout-Analysis

## Project Overview

This project analyzes municipal voter turnout patterns in Quincy, Massachusetts, with the goal of identifying registered voters who may be at higher risk of not participating in local elections. Using an L2 voter file containing 33,315 records and 900 original variables, the analysis includes data cleaning, feature engineering, exploratory analysis, model comparison, and outreach-risk segmentation.

We compared logistic regression, random forest, gradient boosting, and XGBoost classifiers. The final reduced XGBoost model used 18 demographic, socioeconomic, political, residential, and geographic predictors and achieved approximately 0.803 ROC-AUC, 77.7% accuracy, and 89.9% recall for municipal non-voters.

An expanded XGBoost model that included prior voting history and eligibility-adjusted turnout measures achieved higher predictive performance, but its results were dominated by previous participation. Because the project aimed to produce interpretable and actionable outreach insights, the reduced model was selected for the main analysis.

The final model grouped voters into four predicted non-voting risk categories and identified younger voters, non-partisan voters, renters or voters with lower modeled homeownership probability, newer residents, and several represented precincts as potential outreach priorities.

This project is intended as an outreach-prioritization framework rather than a causal explanation of voting behavior. Future work could incorporate individual-level 2025 turnout data, full coverage of Quincy’s 31 precincts, subgroup calibration analysis, and randomized outreach experiments.
