# Support-Vector-Regression-Risk-Quadrangle-Framework-Case-Studies

The paper Support Vector Regression: Risk Quadrangle Framewor introduced the Support Vector Regression (SVR) is a widely used machine learning technique. The Risk Quadrangle (RQ) framework provides a unified interpretation of SVR through four interconnected stochastic functionals—error, regret, risk, and deviation—linked by a common statistic. Within this framework, the ε-SVR and ν-SVR formulations correspond to the minimization of the Vapnik error and the Conditional Value-at-Risk (CVaR) norm. These measures define quadrangles whose statistics equal the average of two symmetric conditional quantiles. Moreover, ν-SVR can be viewed as a form of Distributionally Robust Regression (DRR).

**Overview**

Replicated the theoretical results in Support Vector Regression: Risk Quadrangle Framework by Malandii and Uryasev. Implemented the formulations in Gurobi instead of the PSG solver used in the original case study. To validate the theoretical equivalence and computational performance, conducted experiments on multiple datasets: a simple one-dimensional linear model with Laplace noise, a 10-dimensional uniform independent model, a 10-dimensional multivariate normal model with correlated features. The results confirm the consistency between the theoretical risk quadrangle interpretation and the optimization-based implementation. Finally, we discuss some potential methods that could enhance the results and also introduce how to build the non-linear SVR by applying the kernel-trick.

**Key Concepts**

ε-SVR → minimizes Vapnik ε-insensitive loss

ν-SVR → equivalent to minimizing a CVaR-based norm

Risk Quadrangle → connects regression with:

Quantile-based risk measures, Symmetric conditional quantiles, Distributionally Robust Regression (DRR) → ν-SVR can be interpreted as a DRO problem

**Implementation**

Reimplemented the SVR formulations using Gurobi (instead of the PSG solver used in the original paper)

Formulated SVR as a convex optimization problem

Verified:

Theoretical equivalence

Numerical consistency

**Experiments**

<img width="400" height="200" alt="image" src="https://github.com/user-attachments/assets/0c255bfd-659c-453c-abb0-a6d01c836a5d" />



**Result**

<img width="400" height="200" alt="image" src="https://github.com/user-attachments/assets/728a57fe-7a40-4a24-8210-350eaf12ec28" />




**Tech**

Python, Gurobi Optimizer, Portfolio Safeguard (PSG)



**Key Words**: Support Vector Regression, Risk Quadrangle Framework, CVaR (Conditional Value-at-Risk)

**Reference**:
A. Malandii and S. Uryasev, “Support vector regression: Risk quadrangle framework,” arXiv preprint arXiv:2212.09178, December 3 2024. [Online]. Available: https://arxiv.org/abs/2212.09178
