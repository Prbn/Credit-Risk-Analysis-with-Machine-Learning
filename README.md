# Credit-Risk-Analysis-with-Machine-Learning

This project reviews the process of performing credit risk analysis using machine learning, delving into various methods, their mathematical foundations, and practical applications for predicting loan default risk.

This project provides an in-depth analysis of credit risk, focusing on predicting the likelihood of loan default using machine learning models. It explores key financial concepts like creditors, borrowers, and types of loans, to Mathematical concepts to the implements various models including Logistic Regression, Random Forest, and Decision Trees to assess and mitigate credit risk. The notebook also features data visualizations to enhance understanding of the model performance and insights from the data.

# Credit Risk Analysis

This project explores credit risk, a critical concept in the financial industry, and provides an analysis to understand the likelihood of a borrower defaulting on a loan. The Jupyter Notebook uses Python to perform credit risk analysis and includes several key concepts and techniques to assess risk.

## Project Overview

**Credit Risk**

Credit risk is a critical concept in the financial industry, representing the likelihood that a borrower will fail to repay a loan, causing the lender to suffer losses. Understanding credit risk is essential for lenders to protect themselves from potential defaults and financial crises.


### Key Concepts in Credit Risk

1.  **Creditors and Borrowers**:

    *   **Creditor (Lender)**: Provides goods, services, or money to a borrower.

    *   **Borrower (Debtor)**: Receives goods, services, or money and is obligated to repay the lender.


2.  **Types of Loans**:

    *   **Credit Cards**: Allow borrowers to spend up to a certain limit, which must be repaid with interest.

    *   **Home Ownership Loans**: Borrow money against the equity in a home, with the property serving as collateral.

    *   **Asset Financing**: Companies obtain equipment and pay for its use over time rather than upfront.


3.  **Credit Risk**:

    *   **Definition**: The probability that a borrower will not repay their loan.

    *   **Consequences for Lenders**: Loss of principal and interest, and incurring collection costs.

    *   **Default**: The event of a borrower failing to make required payments.



### Mitigating Credit Risk

1.  **Collateral**: Assets pledged by the borrower to cover the debt in case of default.

2.  **Risk-Based Pricing**: Higher interest rates for borrowers with higher credit risk.


### Importance of Accurate Credit Risk Assessment

*   **Financial Crises**: Poor assessment of credit risk can lead to significant financial crises, as seen in the 2008 global financial crisis. This crisis was fueled by high default rates on subprime mortgages, leading to the collapse of major financial institutions and widespread economic impact.


### Case Study: The 2008 Financial Crisis

*   **Low Interest Rates**: Encouraged increased mortgage lending.

*   **High Mortgage Approval Rates**: Led to higher housing prices and increased borrowing against home equity.

*   **Subprime Borrowers**: High-risk borrowers defaulted, causing mortgage-backed securities to lose value.

*   **Bank Failures**: Institutions like Lehman Brothers and Bear Stearns went bankrupt, while others required government bailouts.


### Conclusion


Credit risk management is vital for the stability of the financial system. Lenders must accurately assess and mitigate credit risk to prevent defaults and protect against financial losses. The 2008 financial crisis serves as a stark reminder of the importance of prudent credit risk assessment and management.

---

## Understanding **Expected Credit Losses (ECL)**

Lenders understand that every loan comes with some degree of credit risk, leading to both expected and unexpected credit losses. Expected losses are predictable and factored into lending decisions, while unexpected losses arise from unforeseen adverse economic conditions.


### Key Concepts in Expected Credit Losses

1.  **Expected Loss (EL)**: The anticipated amount a lender might lose from a borrower defaulting.

2.  **Unexpected Loss**: Losses resulting from unexpected adverse economic conditions, though rare, can be severe.


### Components of Expected Loss

Expected Loss is calculated using three main components:

1.  **Probability of Default (PD)**: The likelihood that a borrower will default on their loan.

2.  **Loss Given Default (LGD)**: The proportion of the loan that cannot be recovered once the borrower defaults.

3.  **Exposure at Default (EAD)**: The total value the lender is exposed to when the borrower defaults.


### Calculation of Expected Loss

The formula for calculating Expected Loss (EL) is:

$$
EL = PD \times LGD \times EAD
$$


### Example Calculation

#### Scenario:

*   A borrower purchases a house for \$500,000.
*   The lender funds 80% of the purchase price.
*   The borrower has repaid \$40,000.
*   Empirical evidence shows a default rate of 25\% (1 in 4 homeowners default).
*   If the borrower defaults, the house can be sold for \$342,000.

#### Steps to Calculate Expected Loss:

1.  **Calculate EAD**:
   
$$
\text{Loan Amount}=80\% \times \$500,000 = \$400,000 \\
\text{Outstanding Balance} = \$400,000−\$40,000 = \$360,000 \\
\text{EAD} = \$360,000
$$   

3.  **Determine PD**:

$$
\text{PD} = 25\%
$$

3.  **Calculate LGD**:

$$
\text{Recoverable Amount} = \$342,000 \\
\text{Remaining Loss} = \$360,000 - \$342,000 = \$18,000 \\
\text{LGD} = \frac{$18,000}{\\$360,000} = 5\\%
$$

4.  **Calculate Expected Loss**:

$$
EL = PD \times LGD \times EAD \\
EL = 25\% \times 5\% \times \$360,000 \\
EL = 0.25 \times 0.05 \times \$360,000 \\
EL = \$4,500 \\
$$

### Conclusion

The Expected Loss of \$4,500 indicates the anticipated loss the lender might face from this specific loan, based on the given PD, LGD, and EAD. Accurately estimating these components is crucial for lenders to manage credit risk effectively and ensure financial stability.

## Key Sections
1. **Creditors and Borrowers**: Explanation of the roles of creditors (lenders) and borrowers (debtors).
2. **Types of Loans**: Covers different loan types, including credit cards.
3. **Risk Assessment**: Practical examples of how to assess credit risk based on borrower data.
4. **Modeling**: Application of machine learning models to predict loan defaults.

## Requirements
To run this notebook, you will need to have the following libraries installed:
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

You can install the required libraries using:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

## Running the Analysis
1. Clone this repository.
2. Open the notebook using Jupyter or any compatible IDE.
3. Run each cell to see the results of the credit risk analysis.

## Models Used

The following models are implemented in the notebook:
- Logistic Regression
- Random Forest
- Decision Trees

Each model is trained on a dataset of borrower characteristics to predict the likelihood of default.

## Visualization

The notebook also includes several visualizations that provide insights into the data and model performance, such as:
- ROC Curves
- Confusion Matrices
- Feature Importance

## Conclusion

This analysis aims to equip financial professionals and data scientists with the tools to better understand and manage credit risk.

Feel free to explore the notebook and improve upon the models and analysis.

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
