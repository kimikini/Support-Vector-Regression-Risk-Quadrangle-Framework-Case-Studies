# Support-Vector-Regression-Risk-Quadrangle-Framework-Case-Studies
The paper Support Vector Regression: Risk Quadrangle Framewor introduced the Support Vector Regression (SVR) is a widely used machine learning technique. The Risk Quadrangle (RQ) framework provides a unified interpretation of SVR through four interconnected stochastic functionals—error, regret, risk, and deviation—linked by a common statistic. Within this framework, the ε-SVR and ν-SVR formulations correspond to the minimization of the Vapnik error and the Conditional Value-at-Risk (CVaR) norm. These measures define quadrangles whose statistics equal the average of two symmetric conditional quantiles. Moreover, ν-SVR can be viewed as a form of Distributionally Robust Regression (DRR).

**Overview**

This project reproduces and extends the results from the paper
“Support Vector Regression: Risk Quadrangle Framework” by Malandii and Uryasev.

Support Vector Regression (SVR) is reinterpreted under the Risk Quadrangle (RQ) framework, which unifies four stochastic functionals:

Error

Regret

Risk

Deviation

These components are linked through a common statistic and provide a risk-based interpretation of regression models.

**Key Concepts**

ε-SVR → minimizes Vapnik ε-insensitive loss

ν-SVR → equivalent to minimizing a CVaR-based norm

Risk Quadrangle → connects regression with:

Quantile-based risk measures

Symmetric conditional quantiles

Distributionally Robust Regression (DRR)
→ ν-SVR can be interpreted as a DRO problem

I**mplementation**

Reimplemented the SVR formulations using Gurobi (instead of the PSG solver used in the original paper)

Formulated SVR as a convex optimization problem

Verified:

Theoretical equivalence

Numerical consistency

**Experiments**

To validate the framework, experiments were conducted on:

1D Linear Model

Laplace noise (heavy-tailed distribution)

10D Independent Model

Uniformly distributed features

10D Correlated Model

Multivariate normal distribution



**Tech Stack**

Python

Gurobi Optimizer

Portfolio Safeguard (PSG)



**Key Words**: Support Vector Regression, Risk Quadrangle Framework, CVaR (Conditional Value-at-Risk)

**Reference**:
A. Malandii and S. Uryasev, “Support vector regression: Risk quadrangle framework,” arXiv preprint arXiv:2212.09178, December 3 2024. [Online]. Available: https://arxiv.org/abs/2212.09178
