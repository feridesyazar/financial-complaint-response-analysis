# 💳 Financial Complaint & Response Analysis

*Financial Services Analytics | Binary Classification*

**Python · Pandas · Matplotlib · Scikit-learn · Logistic Regression**

## About the Project

How can financial-services teams learn from consumer complaints, and can structured complaint information help predict a company's **recorded response category**?

This Data Science case study uses public records from the **Consumer Financial Protection Bureau (CFPB)**. It combines **Exploratory Data Analysis (EDA)** with an interpretable **Logistic Regression** classifier to identify complaint patterns and evaluate reported closure outcomes.


## Business Questions

- Which financial products and issues receive the most reported complaints?
- How are company response categories distributed?
- Which products show higher shares of **reported relief** among closed complaints?
- Can a classifier predict reported relief more usefully than a simple baseline?

## Analysis & Model Results

The notebook explores complaint frequencies and company responses, then applies **One-Hot Encoding** and **Logistic Regression**. A **stratified random 80/20 train-test split** is used, and the model is compared against a majority-class baseline.

| Evaluation metric | Logistic Regression | Baseline |
|---|---:|---:|
| Macro F1 | 0.575 | 0.390 |
| Accuracy | 57.5% | 63.9% |

These are the **saved notebook run's results**. They may differ when the data source or sample changes. The model improves Macro F1 over the baseline but has lower overall accuracy; these results **do not establish production-ready predictive performance**.

## Business Insights

Complaint patterns can help financial-services teams prioritize **process reviews, recurring issue investigations, and response-category analysis**. Model results can guide further experimentation, but they are **not suitable for automated decisions about individual consumers**.

**Important limitations:** CFPB complaint records are not representative of all customers. A company's reported closure category is **not** a measure of customer satisfaction, and complaint counts are not rates adjusted for institution size or customer base.


## Next Steps

Validate the model on later time periods, examine false positives and false negatives, and investigate whether additional reliable data improves performance.
