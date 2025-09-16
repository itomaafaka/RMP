# BondsRisk — процентный риск облигационного портфеля РФ (2014–2025)

**Цель.** Реплицируемый пайплайн: кривая доходности → PCA → ARIMA/(E)GARCH → VaR/ES (в т.ч. FHS) → стресс-сценарии → ML (логистическая регрессия нарушений VaR).

## Стек
Python 3.11.13 (venv). Пакеты: numpy, pandas, scipy, matplotlib, seaborn, plotly, statsmodels, pmdarima, arch, cvxpy, nelson-siegel-svensson, scikit-learn, jupyterlab, xgboost.

## Структура
data/{raw,processed} • notebooks • src (curve/pca/ts/garch/risk/stress/ml) • reports/{figures,tables} • configs • docs • references • tests

## Развёртывание
```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt MD
