# Collateral_Haircut_Calculator
 
## Executive Summary
In banking, ensuring loans are securely matched by collateral is vital to prevent financial exposure. This project delivers an automated risk application that calculates risk-adjusted collateral values in real time.
By automating the data pipeline, the tool eliminates manual lookup issues and protects the desk from human error. It evaluates user inputs for the collateral and automatically applies the total haircut percentage, based on precise foreign exchange (FX) penalty buffers for cross-currency trades, to calculate the maximum eligible loan. Ultimately the calculator ensures strict regulatory compliance, protects firm liquidity and significantly improves data integrity.

## Visual Preview
![Collateral Haircut Calculator Preview]()

## Problem Statement
In banking ensuring the reconcilliation of loans to collateral is critical in preventing financial exposure. Analysts are frequently required to cross reference security lists against complex currency haircut grids. Manual intervention introduces a high probability of human error.

## Objectives
* **Accelerate Processing** - Modernise the workflow to enable near instantaneous loan to collateral calculations.
* **Mitigate Risk** - Reduce human intervention by automating the cross referencing process.
* **Strict controls** - Ensure 100% compliance with Bank of England Standards.

## Technical Highlights

### Multi Dimensional Matrix
Engineered a two dimensional grid mapping system to handle cross currency transactions, based directly on the Bank of England Sterling Monetary Framework (See figure 2.0). By evaluating the Currency of Lending against the Currency of Collateral, the tool dynamically scales the entire regulatory matrix and penalties are calculated for a currency mismatch.

![]()

*Figure 2.0: The official Bank of England prudental schedule used as the source architecture for the calculator's backend two dementional lookup matrix*
### 
```excel

```
### Workflow Automation using Macros
Developed process automation scripts to eliminate repetitive manual tasks. Using macros the tool allows users to reset transaction inputs and reset the calculator view with a click of a button, reducing operational friction.

## Financial Calculations

### 1. Total Haircut Percentage
Total Haircut Percentage (%) = Baseline Asset Risk (%) + FX Mismatch Penalty (%)
* Ensures that if a loan is in GBP but the collateral is in USD, the foreign exchange volatility buffer is automatically added to the baseline asset risk.

### 2. Haircut Applied Dollar Value
Haircut Applied Value = Collateral Market Value x Total Haircut Percentage.

### 3. Maximum Eligible Loan
Maximum Eligible Loan = Collateral Market Value - Haircut Applied Value.

## Operational Impact & Conclusion
By replacing a manual error prone spreadsheet workflow with a dynamic calculation tool, this project successfully eliminated the root cause of data exceptions at the UI level. The resulting tool helps to ensure data integrity and directly mitigates institutional financial exposure.

