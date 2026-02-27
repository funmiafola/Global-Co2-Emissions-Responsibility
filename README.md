GLOBAL CO2 EMISSIONS RESPONSIBILITY : Total vs Per-Capita vs Historical Accountability Dashboard

# Project Overview 
This project presents an interactive Power BI dashboard that explores global CO2 emissions responsibility from different perspectives. It compares total national emissions, emissions per capita, historical cumulative emissions, and Predictive modelling and future forecasts.

The objective is to examine climate accountability and fairness by analysing how responsibility differs depending on whether emissions are viewed from total output, individual contribution, or historical accumulation.


The dashboard supports evidence-based climate policy discussions, sustainability strategy development, and public awareness by transforming complex environmental datasets into structured, interactive visual insights for both technical and non-technical audiences.

# Dataset Content
The dataset used in this project was obtained from Our World in Data (OWID), which compiles global CO2 emissions statistics from trusted research sources such as the Global Carbon Project.

The dataset includes country-level data across multiple years.

Key variables used in this project:
Country – Name of the country
Year – Reporting year
 CO2 (Total emissions) – Annual national emissions
CO2 per capita – Emissions per person
Population – Used for scaling and comparison
GDP - Used for predictive modelling
Cumulatice CO2- Historical emissions since industrialisation

The dataset covers several years, which allows the analysis of historical trends, cumulative emissions and Predictive modelling.

The data is publicly available, licensed for reuse and contain no personal or sensititive information.  

# Business Requirements

The dashboard was designed to answer the following key policy and sustainability questions:
Which countries contribute the most to global CO2 emissions today? 
How have global emissions changed since 1990?
How does per-capita responsibility differ from total national emissions?
Which countries hold the greatest historical accountability?
Do demographic and economic factors significantly explain emissions variation?
What are projected global emissions trend up to 2030?



# Hypothesis and how to validate?

H1: Global CO2 emissions have increased significantly since 1990

Validation: This will be evaluated using : Time-Series trend analysis, Linear Regression forecastion model and Percentage growth calculation
Result: Confirmed. Emissions increased by approximatley 68.6% since 1990

H2: Countries with large populations account for higher total emissions but do not necessarily rank highest in per-capita emissions.

Validation: This will be analysed using : Pearson Correlation (Population vs Total CO2) and Scatter plot with responsibillity quadrants

Result:Strong positive correlation (r = 0.824, p < 0.001).
However, high population countries do not always rank highest in per-capita emissions.


H3: Developed countries tend to have higher CO2 emissions per capita compared to developing countries.

Validation: This will be assessed by: Independent t-test and per- capita ranking comparison.

Result: Result:
T-statistic = 1.90
p-value = 0.098

The difference was not statistically significant at the 5% level within the restricted high-emitter subset. However, descriptive analysis suggests developed economies appear more frequently among extreme per-capita emitters.

H4: Countries with the highest historical cumulative emissions are not always the same as those with the highest current annual emissions.

Validation: This will be examined  using: Cumulative emission ranking and Comparison with current annual emissions.

Result: Confirmed.
The United States leads cumulative emissions historically, while China leads current annual emissions.

Predictive Modelling

Two regression models were developed to assess emissions drivers


# Model A – Global Emissions Forecast

A simple linear regression model was developed to forecast global emissions trends.

Results:

R² = 0.964

Annual increase ≈ 515 million tonnes

Projected continued growth to 2030

This indicates strong historical trend persistence.

# Model B1 – Population Only Regression

Predictor: Population
Target: Total CO2

# Results:

MAE = 89.68

RMSE = 166.91

R² = -0.429

The negative R² indicates poor predictive performance when using population alone.

# Model B2 – Multiple Linear Regression

Predictors:

Population

GDP

Results:

MAE = 99.72

RMSE = 153.94

R² = 0.751

The multi-factor model explains 75% of emissions variation, demonstrating that economic activity significantly amplifies emissions beyond population effects.

# Key Insight

Emissions responsibility is multidimensional.
Population contributes to scale, but GDP and industrial structure significantly influence total emissions levels.




# Research Methodology Rationale

The following methodologies were selected:

Exploratory Data Analysis (EDA) to understand trends and distributions

Pearson correlation to assess linear relationships

Independent t-test for group comparison

Linear regression for forecasting

Multiple regression for predictive modelling

Model evaluation using MAE, RMSE, and R²

These techniques were selected because:

They align with business requirements

They are statistically interpretable

They support both descriptive and predictive insight


# Project Plan
Planning
    Define business case
    Identify datasets
    Establish hypotheses
Data Collection
    Source OWID dataset
    Verify licensing and governance
Data Processing and Transformation
    Clean missing values
    Filter relevant years
    Create derived metrics
EDA Analysis
    Trend analysis
    Responsibility comparisons
    Growth calculations

Predictive Modelling 

Interpretation and Dashboarding

# Dashboard Development
    Build visualisations in BI tool https://app.powerbi.com/groups/me/reports/a8a78e7c-8d4c-47d3-a62a-acc68d39996d/fa22ae502632d89b08d0?ctid=c233c072-135b-431d-af59-35e05babf941&experience=power-bi
The dashboard consists of four analytical pages:

# Page 1 – Global Overview

KPI Cards

Global trend line

Emissions growth metric

# Page 2 – National Responsibility

Top 10 emitters bar chart

Total vs Per-Capita scatter plot

Narrative explanation

# Page 3 – Per-Capita Responsibility

Highest per-capita ranking

Development status comparison

# Page 4 – Historical & Predictive Modelling  

Cumulative emissions comparison

Forecast to 2030

Model comparison chart

Coefficient impact chart


# Mapping Business Requirements to Visualisations
Business Requirement -	Visualisation
Top emitters -	Bar chart (Top 10 countries)
Global trend -	Time-series line chart
Total vs per-capita	- Scatter plot
Historical responsibility -	Cumulative emissions bar chart
Model comparison -	R² comparison chart
Forecasting	Line  - projection to 2030



# Data Management
Raw data stored in DataSet/Raw/

Cleaned datasets stored in DataSet/Cleaned/

Exported dashboard and modelling outputs stored in DataSet/Exported/

Data cleaning steps included:

Removing null values

Filtering relevant years
Creating derived metrics (growth rates, clasification field)


# Ethical Considerations

No personal data was used.

Data sourced from publicly available research.

Interpretation acknowledges that emissions responsibility debates involve ethical and geopolitical complexity.

Limitations in GDP completeness were transparently addressed.


# Use of Generative AI

Generative AI was used to assist with:

Code optimisation in Python

Structuring regression workflows

Debugging modelling errors

Structuring the documetation 

Improving dashboard narrative clarity

All outputs were reviewed, tested, and validated manually.


# Unfixed Limitations

GDP missing values reduced modelling sample size.

Linear regression assumes linearity and does not account for structural breaks.

Forecast model does not incorporate policy interventions or non-linear climate transitions.

# Development Roadmap

Challenges encountered:

Missing GDP values

Regression model underperformance

Aggregation issues in Power BI

# Solutions:

Switched to latest-available-year modelling

Compared multiple regression approaches

Created DAX measures to prevent coefficient aggregation

# Future improvements:

Add regional-level modelling

Implement time-series forecasting models (ARIMA)

Add interactive model parameter 

Standardization (Scaling ) needed for coefficients


# Main Libraries Used

pandas – Data cleaning and transformation

numpy – Numerical calculations

scipy – Hypothesis testing

scikit-learn – Regression modelling

matplotlib – Visual exploration

Power BI – Interactive dashboard development

# Credits

Data:
Our World in Data (OWID) – CO2 Emissions Dataset

# Tools:
Microsoft Power BI
Python (Pandas, Scikit-learn, SciPy)



Acknowledgements

Thanks to my facilitator  who provided feedback on the project.
