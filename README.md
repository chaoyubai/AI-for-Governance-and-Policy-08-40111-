# Algorithmic Bias Replication: ProPublica COMPAS Analysis
original study:
https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing/
## Project Overview
This repository contains the replication of the 2016 ProPublica investigation, "Machine Bias," which analyzed the racial disparities in the COMPAS (Correctional Offender Management Profiling for Alternative Sanctions) risk assessment tool used in the U.S. judicial system. 

The goal of this project is to verify the core findings—specifically the disparate False Positive Rates (FPR) between African-American and Caucasian defendants—and to assess the implications of algorithmic prioritization in public policy.

## File Structure
- `reproduce.ipynb`: The primary Jupyter Notebook containing data preprocessing, logistic regression analysis, and fairness metric calculations.
- `requirements.txt`: A list of Python libraries required to run the replication.
- `compas-scores-two-years.csv`: The original dataset obtained from ProPublica’s GitHub repository.

## Installation & Setup
To ensure a consistent environment, it is recommended to use a virtual environment. You can install the necessary dependencies using the following command:

pip install -r requirements.txt

Execution Instructions (Single Execution)
The entire replication process is encapsulated within reproduce.ipynb.

Ensure compas-scores-two-years.csv is in the same directory as the notebook.

Open the notebook in a Jupyter environment.

Select "Run All" cells.

## Key Findings
Our replication successfully confirmed the racial bias identified in the original study:

Odds Ratio: Controlling for actual recidivism and priors, African-American defendants are approximately 1.62 times more likely to receive a higher score than Caucasian defendants.

Fairness Gap: The False Positive Rate (FPR) for African-American defendants (42.34%) is nearly double that of Caucasian defendants (22.01%).