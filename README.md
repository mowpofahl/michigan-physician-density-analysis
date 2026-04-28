# Physician Density and Socioeconomic Disparities in Michigan ZIP Codes (1990–2021)

Analysis of physician density disparities across Michigan ZIP codes by income level and demographic characteristics, using longitudinal data from 1990–2021.

## Research Questions

1. How has physician density changed across Michigan ZIP codes between 1990 and 2021, and does it differ by income level?
2. Which demographic characteristics — specifically poverty rate, median family income, disadvantage index, proportion Hispanic, and proportion non-Hispanic Black — are most strongly associated with low physician density across Michigan ZIP codes in 2021?

## Key Findings

- Highest-income ZIP codes had consistently higher physician density than all other income groups across the entire 31-year period.
- The gap between the highest and lowest income quartiles roughly doubled between 1990 and 2021, with no lasting progress toward closing it.
- Median family income was the strongest predictor of physician density (r = 0.23, p < 0.001), with proportion non-Hispanic Black second (r = 0.17, p < 0.001).
- Poverty rate showed near-zero correlation with physician density, likely due to high multicollinearity with the disadvantage index (r = 0.92).

## Tools & Methods

- Python (pandas, scipy, matplotlib)
- Pearson correlation analysis
- Income quartile classification via pd.qcut
- Robustness checks: alternative income grouping, alternative year (2018), multicollinearity check

## Data Sources

- [NaNDA Healthcare Services by ZCTA, 1990–2021](https://doi.org/10.3886/ICPSR38559.v1) — physician density measures by ZIP code
- [NaNDA Socioeconomic Status and Demographic Characteristics of ZCTAs, 1990–2022](https://doi.org/10.3886/ICPSR38528.v6) — income, poverty, and demographic variables
