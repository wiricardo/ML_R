# Machine Learning with R

Machine Learning project **by Wiricardo** for credit score prediction using R and Quarto. Compares Linear Regression vs Random Forest models with customer data.

## Overview

This project predicts **customer credit scores** based on: 
- Annual Income 
- Estimated Savings
- Preferred Category (product preference)

Dataset: Mall Customers Enhanced

## Models Implemented

**Linear Regression (3 variants)** - Model 1: Annual Income only - Model 2: Annual Income + Estimated Savings - Model 3: All features including Preferred Category

**Random Forest** - 500 trees, optimized hyperparameters - Better performance handling non-linear relationships

## Results

| Model                       | RMSE  | R²   |
|-----------------------------|-------|------|
| Linear Regression (Model 3) | \~80 | 0.75 |
| Random Forest               | \~40  | 0.94 |

Random Forest significantly outperforms linear regression due to multicollinearity between income and savings (correlation: 0.81).

## Project Structure

```         
ML_R/
├── Final_R.qmd              # Main analysis notebook
├── Mall_Customers_Enhanced.csv
├── m1_plot.rds              # Linear regression plots
├── m2_plot.rds
├── m3_plot.rds
├── rf_plot.rds              # Random forest plot
└── *_metrics.rds            # Model performance metrics
```

## Key Findings

-   High multicollinearity between Annual Income and Estimated Savings (0.81)
-   Linear relationships exist but with curvature at extreme values
-   Random Forest handles non-linearity better than linear regression
-   Feature engineering with dummy variables improves model performance

## Contact

For suggestions, bug reports, or collaboration:\
**GitHub profile** → [wiricardo](https://github.com/wiricardo)

## License

This project is licensed under the **MIT License**.\
See the [LICENSE](LICENSE) file for more details.
