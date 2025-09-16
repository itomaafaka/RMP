# Interest Rate Risk of Russian Bond Portfolio

Reproducible pipeline for interest rate risk analysis.  
Methods: 
→ yield curve 
→ PCA 
→ ARIMA/(E)GARCH 
→ VaR/ES (incl. FHS) 
→ stress scenarios 
→ ML (logistic regression for VaR breaches).

---

## Tech Stack

Language / runtime:  
Python 3.11.13 (venv)

Core packages:  
- `numpy`, `pandas`, `scipy` — core math and statistics  
- `matplotlib`, `seaborn`, `plotly` — visualization  
- `statsmodels`, `pmdarima`, `arch` — time series, ARIMA, (E)GARCH  
- `cvxpy`, `ecos`, `osqp` — optimization & risk models  
- `nelson-siegel-svensson` — yield curve fitting  
- `scikit-learn`, `xgboost` — machine learning (PCA, logistic regression, boosting)

Workflow:  
JupyterLab, VS Code  