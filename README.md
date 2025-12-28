# python-bank-reconciliation

# Bank vs Ledger Reconciliation Automation (Python)

## Overview
This project automates the reconciliation process between a bank statement and an internal company ledger using Python.

It compares transactions from both sources, identifies matches, and highlights reconciliation breaks such as missing or unmatched transactions. The final output is generated as an Excel report for easy business review.

---

## Features
- Automated bank vs ledger reconciliation
- Exact matching on transaction date and amount
- Date tolerance matching (±1 day) to handle posting delays
- Amount tolerance matching (±₹5) to handle rounding or charge differences
- Clear classification of reconciliation status
- Excel output with detailed and summary views

---

## Tools & Libraries Used
- Python
- Pandas
- OpenPyXL
- Jupyter Notebook

---

## Reconciliation Logic
1. Load bank and ledger data from Excel files
2. Standardize column names for consistency
3. Perform exact matching on date and amount
4. Apply date tolerance (±1 day) for delayed postings
5. Apply amount tolerance (±₹5) for minor value differences
6. Classify transactions as:
   - Matched
   - Missing in Bank
   - Missing in Ledger
7. Generate Excel output with:
   - Reconciliation_Details sheet
   - Reconciliation_Summary sheet

---

## Output
The reconciliation result is generated as a single Excel file containing:
- Detailed transaction-level reconciliation
- Summary of matched and unmatched transactions

---

## Use Cases
- Bank reconciliation teams
- Finance and operations teams
- Custody and settlement operations
- AML and transaction monitoring support functions

---

## How to Run
1. Install dependencies:
   pip install -r requirements.txt
2. Open Jupyter Notebook:
   jupyter notebook
3. Run reconciliation.ipynb

---

## Notes
This project uses dummy data for demonstration purposes and is intended to showcase reconciliation automation logic.
