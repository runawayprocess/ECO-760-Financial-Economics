# ECO-760-Financial-Economics
projects for a financial economics course

ECON760_SBA
- Dataset: national SBA loan file (CSV on Drive); target = default (0/1).
- Preprocessing: leakage variable removal, 75/25 train–test split, z-score scaling with StandardScaler, selected feature engineering.
- Modeling: LogisticRegression baseline, nonlinear baselines with GradientBoostingClassifier / HistGradientBoostingClassifier, additional trials with BernoulliNB.
- Feature selection: SequentialFeatureSelector inside an sklearn Pipeline, comparative specs with and without engineered features.
- Validation: cross-validation, regularization tuning; evaluation via ROC curve and AUC, confusion matrix, and classification report.
- Reporting: side-by-side model performance, variable importance discussion, robustness checks against simpler specs.

Homeworks #1/#3/#4:
- Homework 1 demonstrates core stats and simulation skills (NumPy/Pandas for descriptive stats, winsorization, Poisson/Binomial sampling; bootstrap SEs, Matplotlib/Seaborn histograms with KDE) and finishes with basic portfolio analytics using yfinance data (returns, covariances, two-asset minimum-variance weights, correlation SE). Homework 3 extends to asset pricing and optimization: CAPM beta estimation via statsmodels OLS on excess returns, cross-sectional CAPM tests, and mean–variance efficient frontiers solved with scipy.optimize.minimize, with risk–return visualizations. Homework 4 focuses on three equities (CAKE, PLAY, GRND) to compute returns and covariance matrices and compare constrained vs unconstrained efficient frontiers, again optimizing with scipy.optimize.minimize and plotting frontier curves and optimal weights.
