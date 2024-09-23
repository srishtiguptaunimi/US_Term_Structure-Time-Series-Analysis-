# Project Title: Time Series Analysis of US Term Structure

## Overview
This repository contains a comprehensive analysis of the US Term Structure using time series econometric techniques. The primary objective is to test for unit roots in various maturity series and examine the cointegration relationships among them. The methodologies employed include the Augmented Dickey-Fuller (ADF) test for unit roots and the Johansen test for cointegration.

## Table of Contents
- [Project Description](#project-description)
- [Data](#data)
- [Methodology](#methodology)
  - [Unit Root Testing](#unit-root-testing)
  - [Cointegration Testing](#cointegration-testing)
  - [Engle-Granger Methodology](#engle-granger-methodology)
- [Results](#results)
- [Conclusion](#conclusion)
- [Appendix](#appendix)

## Project Description
This project aims to analyze the term structure of interest rates in the United States by testing for unit roots and cointegration among various maturity series: m1, m2, m3, m6, Y1, Y2, Y3, Y4, and Y5. The analysis provides insights into the long-term relationships between these interest rates and evaluates whether they align with the Expectations Hypothesis.

## Data
The dataset used in this analysis includes interest rates for different maturities sourced from reliable financial databases. The series analyzed are:
- m1
- m2
- m3
- m6
- Y1
- Y2
- Y3
- Y4
- Y5

## Methodology

### Unit Root Testing
The presence of unit roots in the time series was assessed using the ADF test. The following steps were followed:
1. **Series Selection**: The series m1, m2, m3, m6, Y1, Y2, Y3, Y4, and Y5 were tested.
2. **ADF Test Results**: 
   - For m1 at level form: t-statistic = 2.529 (not reject null hypothesis).
   - At first difference: no unit root detected.
   - Similar results were found for other series.

### Cointegration Testing
The Johansen test was conducted to determine the cointegration rank among the selected series:
1. **VAR Model Estimation**: Appropriate lag order was selected based on Information Criteria (Schwarz Criterion).
2. **Johansen Test Results**:
   - λtrace indicated 8 cointegration relationships.
   - λmax confirmed similar findings.
   - Conclusion: The series exhibit long-run relationships.

### Engle-Granger Methodology
For the pair of rates m1 and Y1:
1. **Testing for Cointegrating Vector**: Both λtrace and λmax suggested one cointegration relation exists between m1 and Y1.
2. **Cointegrating Equation**: The estimated equation is represented as:
   $$ \text{ECM}_t = m_t - 0.9228y_t + 0.3077B_c $$

## Results
The analysis revealed that:
- All tested series have a unit root at level form but are stationary at first difference.
- There are significant long-run relationships among the interest rates analyzed.
- The findings support implications derived from the Expectations Hypothesis, indicating that interest rates are I(1) and cointegrated.

## Conclusion
This project successfully demonstrates the application of time series econometric techniques to analyze the US Term Structure. The results indicate meaningful long-term relationships among different maturity rates and provide evidence consistent with economic theories regarding interest rate behavior.

## Appendix
The appendix contains visual outputs from the analysis:
- **Fig 1**: ADF Unit Root Test (M1)
- **Fig 2**: ADF Unit Root Test for D(m1)
- **Fig 3**: VAR Model Estimation for Lag Selection
- **Fig 4**: Johansen Cointegration Test – λtrace
- **Fig 5**: Johansen Cointegration Test – λmax
- **Fig 6**: Lag Length Criteria for M1 & Y1
- **Fig 7**: Johansen Cointegration Test for Series m1 & y1 – λtrace 
- **Fig 8**: Johansen Cointegration Test for Series m1 & y1 – λmax 
- **Fig 9**: Vector Error Correction Model 

This README serves as a comprehensive guide to understanding the objectives, methodologies, results, and implications of this time series analysis project.

Detailed report of the analysis is attached feel free to reach me for any queries.
Thank You!
