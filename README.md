# Payment-Fraud-Pattern-Analysis

**Tools:** SQL (SQLite) · **Data:** [PaySim](https://www.kaggle.com/datasets/ealaxi/paysim1) synthetic mobile money transactions, 6,362,620 rows · **Author:** Tamara Ndi
## The question
Payment platforms have to approve real payouts quickly and stop fraud before money leaves. Using a month of simulated transactions, I asked:
1. Where and how does fraud show up?
2. Can simple, explainable rules catch more fraud than the existing flag, and what does each rule cost in false alarms?

## The data
Each row is one transaction: type (PAYMENT, TRANSFER, CASH_OUT, CASH_IN, DEBIT), amount, sender and receiver balances before and after, the hour it happened (`step`) and a label marking fraud. The dataset also has a built-in flag (`isFlaggedFraud`), which I used as the baseline.
