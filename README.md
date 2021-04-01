# RoboAdvisor for Retirement Plans

Using AWS Lex and python, I created a RoboAdvisor to help make recommendations for retirement plan investments.

The RoboAdvisor functions with the use of a Lambda function, which outputs a recommendation after analyzing inputs provided by the user. 

## Required Inputs

* User name
* Age
* Investment amount
* Risk level

## Input Validation Requirements

The user provided inputs must be validated according to the following criteria:

* Age should be greater than zero and less than 65
* Investment amount should be equal to or greater than 5000

## Investment Portfolio Recommendations

Once the user provided inputs are validated, the user select a desired risk level. Based on this choice, one of the following recommendations is provided:

* **None:** "100% bonds (AGG), 0% equities (SPY)"
* **Very Low:** "80% bonds (AGG), 20% equities (SPY)"
* **Low:** "60% bonds (AGG), 40% equities (SPY)"
* **Medium:** "40% bonds (AGG), 60% equities (SPY)"
* **High:** "20% bonds (AGG), 80% equities (SPY)"
* **Very high:** "0% bonds (AGG), 100% equities (SPY)"
